AdditionalFamilyMemberContact

```cs
public class AdditionalFamilyMemberContact
{
    public Guid ContactId { get; set; }
    public Contact Contact { get; set; }

    public Guid AdditionalFamilyMemberContactId { get; set; }
    public AdditionalFamilyMember AdditionalFamilyMember { get; set; }
}
```
