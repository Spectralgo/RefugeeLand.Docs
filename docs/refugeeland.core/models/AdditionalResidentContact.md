
# AdditionalResidentContact

```csharp
public class RefugeeContact
{
    public Guid ContactId { get; set; }
    public Contact Contact { get; set; }

    public Guid AdditionalResidentId { get; set; }
    public AdditionalResident AdditionalResident { get; set; }
}
```