# ShelterRequest

```cs
public class ShelterRequest : IAuditable
{
    public Guid Id { get; set; }
    public DateTimeOffset StartDate { get; set; }
    public DateTimeOffset EndDate { get; set; }
    public ShelterRequestStatus Status { get; set; }

    public Guid ShelterId { get; set; }
    public Shelter Shelter { get; set; }

    public Guid RefugeeGroupId { get; set; }
    public RefugeeGroup RefugeeGroup { get; set; }

    public Guid RefugeeId { get; set; }
    public Refugee RefugeeApplicant { get; set; }

    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }
}
```