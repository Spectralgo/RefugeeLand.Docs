# RefugeeSkillSetDocument

```csharp
public class RefugeeSkillSetDocument
{
    public Guid SkillSetId { get; set; }
    public SkillSet SkillSet { get; set; }

    public Guid DocucmentId { get; set; }
    public Document Document { get; set; }

    public Guid RefugeeId { get; set; }
    public Refugee Refugee { get; set; }
}
```