# Pet

```csharp
class Pet
{
        public Guid Id { get; set; }
        public string Name { get; set; }
        public PetType Type { get; set; }
        public PetGender Gender { get; set; }
        public DateTimeOffset BirthDate { get; set; }
        public string AdditionalDetails { get; set; }
        
        [JsonIgnore]
        public IEnumerable<MedicalCondition> MedicalCondition { get; set; }

}
```
