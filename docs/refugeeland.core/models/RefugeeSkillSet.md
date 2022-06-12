# RefugeeSkillSet

```cs
class RefugeeSkillSet
{
	public Guid Id { get; set; }
	public string Name { get; set; }
	public int YearsOfExperience { get; set; }
	public int YearsOfStudy { get; set; }
	public string AdditionalDetails { get; set; }

	public Guid RefugeeId { get; set; }
	public Refugee Refugee { get; set; }

}
```
