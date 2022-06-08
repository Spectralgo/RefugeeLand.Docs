# RefugeeGroup

```csharp
public class RefugeeGroup : IAuditable
{
        public Guid Id { get; set; }
        public string Name { get; set; }
        
        public Guid RefugeeRepresentativeId { get; set; }
        public Refugee RefugeeRepresentative { get; set; }
        
        public DateTimeOffset CreatedDate { get; set; }
        public DateTimeOffset UpdatedDate { get; set; }
        public Guid CreatedBy { get; set; }
        public Guid UpdatedBy { get; set; }
            
        [JsonIgnore]
        public IList<Refugee> Refugees { get; set; }
}
```
