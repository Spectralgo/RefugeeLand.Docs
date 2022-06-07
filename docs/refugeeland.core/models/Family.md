# Family

```csharp
public class Family : IAuditable
{
    public Guid Id { get; set; }
	public string Name { get; set; }

    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }

    [JsonIgnore]
	public IList<Refugee> RefugeeMembers { get; set; }

    [JsonIgnore]
	public IList<Host> HostMembers { get; set; }

    [JsonIgnore]
	public IList<AdditionalFamilyMembers> AdditionalFamilyMembers { get; set; }
}
```
