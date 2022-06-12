# Host

```csharp
class Host 
{
	public Guid Id { get; set; }
	public string FirstName { get; set; }
	public string MiddleName { get; set; }
	public string LastName { get; set; }
	public string AdditionalDetails { get; set; }
	public Gender Gender { get; set; }
	public DateTimeOffset BirthDate { get; set; }
	
    public DateTimeOffset CreatedDate { get; set; }
    public DateTimeOffset UpdatedDate { get; set; }
    public Guid CreatedBy { get; set; }
    public Guid UpdatedBy { get; set; }
	
    [JsonIgnore]
    public IEnumerable<HostContact> HostContacts { get; set; }

    [JsonIgnore]
    public IEnumberable<Shelter> Shelters { get; set; }

    [JsonIgnore]
    public IEnumerable<HostFamilyMembership> HostFamilyMemberships { get; set; }

    [JsonIgnore]
	public IEnumerable<HostLanguage> HostLanguages { get; set; }

    [JsonIgnore]
	public IEnumerable<HostNationality> HostNationalities { get; set; }

    [JsonIgnore]
	public IEnumerable<HostMedicalCondition> HostMedicalConditions { get; set; }

    [JsonIgnore]
    public IEnumerable<HostDocument> HostDocuments { get; set; }

}
```
