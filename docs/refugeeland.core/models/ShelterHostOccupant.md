# ShelterHostOccupant

```csharp
public class ShelterHostOccupant
{
    public Guid ShelterId { get; set; }
    public Shelter Shelter { get; set; }

    public Guid HostId { get; set; }
    public Host Host { get; set; }
}
```
