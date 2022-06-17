# ShelterAdditionalResidentOccupant

```csharp
public class ShelterAdditionalResidentOccupant
{
    public Guid ShelterId { get; set; }
    public Shelter Shelter { get; set; }

    public Guid AdditionalResidentId { get; set; }
    public AdditionalResident AdditionalResident { get; set; }
}
```