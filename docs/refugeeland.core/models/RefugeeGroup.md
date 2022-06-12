# RefugeeGroup

```csharp
public class RefugeeGroup 
{
        public Guid Id { get; set; }
        public string Name { get; set; }

		//One who speaks for the group during negotiations and requests
        public Guid RefugeeRepresentativeId { get; set; }
        public Refugee RefugeeRepresentative { get; set; }
        
        public DateTimeOffset CreatedDate { get; set; }
        public DateTimeOffset UpdatedDate { get; set; }
        public Guid CreatedBy { get; set; }
        public Guid UpdatedBy { get; set; }
            
        [JsonIgnore]
        public IEnumerable<Refugee> Refugees { get; set; }
}
```
