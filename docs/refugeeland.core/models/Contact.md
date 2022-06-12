# Contact

```csharp
public class Contact 
{
    public Guid Id { get; set; }
    public bool IsPrimary { get; set; }
    public ContactType Type { get; set; }
    public string Information { get; set; }
    public string Notes { get; set; }
	
    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }

    [JsonIgnore]
    public IEnumerable<RefugeeContact> RefugeeContacts { get; set; }

    [JsonIgnore]
    public IEnumerable<HostContact> HostContacts { get; set; }	

    [JsonIgnore]
    public IEnumerable<HostContact> AdditionalFamilyMemberContacts { get; set; }	

    [JsonIgnore]
    public IEnumerable<UserContact> UserContacts { get; set; }	
}
```
