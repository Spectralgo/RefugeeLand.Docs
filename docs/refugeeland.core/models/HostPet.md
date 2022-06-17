
# HostPet

```csharp
public class HostPet
{
    public Guid HostId { get; set; }
    public Host Host { get; set; }

    public Guid PetId { get; set; }
    public Pet Pet { get; set; }
}
```