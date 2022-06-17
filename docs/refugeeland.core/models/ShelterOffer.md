# ShelterOffer

```csharp
public class ShelterOffer 
{
    public Guid Id { get; set; }
    public DateTimeOffset StartDate { get; set; }
    public DateTimeOffset EndDate { get; set; }
    public ShelterOfferStatus Status { get; set; }

    public Guid ShelterId { get; set; }
    public Shelter Shelter { get; set; }
	
    public Guid HostId { get; set; }
    public Host Host { get; set; }

    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }

    [JsonIgnore]
    public IList<ShelterRequest> ShelterRequests { get; set; }
}
```
