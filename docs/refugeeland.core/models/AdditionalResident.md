```cs
public class AdditionalFamilyMember
{
	public Guid Id { get; set; }
	public string FirstName { get; set; }
	public string LastName { get; set; }
	public string AdditionalDetails { get; set; }
	public Gender Gender { get; set; }
	public DateTimeOffset BirthDate { get; set; }
	public IList<Languages> Languages { get; set; }
	public IList<Nationality> Nationalities { get; set; }
	
    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }
	
    [JsonIgnore]
    public IEnumerable<AdditionalResidentContact> AdditonalResidentContacts { get; set; }

}
```