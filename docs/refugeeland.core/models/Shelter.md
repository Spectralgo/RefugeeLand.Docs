
```cs
public class Shelter : IAuditable
{
	public Guid Id { get; set; }
	public Guid HostId { get; set; }
	public string ShelterType { get; set; }
	public string Location { get; set; }
	public string AdditionalDetails { get; set; }
	public int MaximumCapacity { get; set; }
	public int BedroomNumber { get; set; } 
	public int SingleBedNumber { get; set; }
	public int DoubleBedNumber { get; set; }
	public int ChildBedNumber { get; set; }
	public int BabyBedNumber { get; set; }
	public bool IsSmokingAllowed { get; set; }
	public bool IsPetAllowed { get; set; }
	public bool IsHandicappedAccessible { get; set; }
	public bool IsVerified { get; set; }
	public bool IsShared { get; set; }
	public string SharedSpaceDetails { get; set; }
	public ShelterStatus Status { get; set; }
	public IList<AllowedPet> AllowedPets { get; set; }
	
    DateTimeOffset CreatedDate { get; set; }
    DateTimeOffset UpdatedDate { get; set; }
    Guid CreatedBy { get; set; }
    Guid UpdatedBy { get; set; }


    [JsonIgnore]
    public IList<ShelterRefugeeOccupant> ShelterRefugeeOccupants { get; set; }
	
    [JsonIgnore]
    public IList<ShelterHostOccupant> ShelterHostOccupants { get; set; }
	
    [JsonIgnore]
    public IList<AdditionalFamilyMemberOccupant> 
	    AdditionalFamilyMemberOccupants { get; set; }
}
```

