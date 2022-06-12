# Family

```csharp
public class Family 
{
    public Guid Id { get; set; }
	public string Name { get; set; }

    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }

    [JsonIgnore]
	public IEnumerable<RefugeeFamilyMembership> RefugeeFamilyMembers { get; set; }

    [JsonIgnore]
	public IEnumerable<RefugeeFamilyMembership> HostFamilyMembers { get; set; }

    [JsonIgnore]
	public IEnumerable<AdditionalFamilyMembership> AdditionalFamilyMembers { get; set; }
}
```
