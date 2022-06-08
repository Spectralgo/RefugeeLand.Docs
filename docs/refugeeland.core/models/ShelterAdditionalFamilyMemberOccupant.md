# ShelterAdditionalFamilyMemberOccupant

```csharp
public class ShelterAdditionalFamilyMemberOccupant
{
    public Guid ShelterId { get; set; }
    public Shelter Shelter { get; set; }

    public Guid AdditionalFamilyMemberId { get; set; }
    public AdditionalFamilyMember AdditionalFamilyMember { get; set; }
}
```
