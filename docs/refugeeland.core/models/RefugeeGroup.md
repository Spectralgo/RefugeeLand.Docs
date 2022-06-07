```cs
public class RefugeeGroup : IAuditable
{
	public Guid Id { get; set; }
	public string Name { get; set; }
	public Refugee Representative { get; set; }

    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }


    [JsonIgnore]
	public IList<Refugee> Refugee { get; set; }
}
```