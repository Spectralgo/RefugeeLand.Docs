# ShelterRefugeeOccupant

```csharp
public class ShelterRefugeeOccupant
{
        public Guid ShelterId { get; set; }
        public Shelter Shelter { get; set; }

        public Guid RefugeeId { get; set; }
        public Refugee Refugee { get; set; }

        public DateTimeOffset StartDate { get; set; }
        public DateTimeOffset EndDate { get; set; }
        public InhabitationStatus InhabitationStatus { get; set; }
}
```
