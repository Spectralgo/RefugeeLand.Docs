# Refugee

```csharp
class Refugee : IAuditable
{
	public Guid Id { get; set; }
	public string FirstName { get; set; }
	public string MiddleName { get; set; }
	public string LastName { get; set; }
	public string CurrentLocation { get; set; }
	public string SkillSets { get; set; }
	public string AdditionalDetails { get; set; }
	public bool IsOpenToWork { get; set; }
	public Gender Gender { get; set; }
	public DateTimeOffset BirthDate { get; set; }
	public IList<Language> Languages { get; set; }
	public IList<Nationality> Nationalities { get; set; }
	public IList<MedicalCondition> MedicalConditions { get; set; }
	
	public Guid FamilyId { get; set; }
	public Family Family { get; set; }

    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }


    [JsonIgnore]
    public IEnumerable<RefugeeContact> RefugeeContacts { get; set; }

}
```
