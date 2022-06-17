# RefugeeGroupMembership
```cs      
public class ShelterRequest
{
	public Guid RefugeeGroupId { get; set; }
    public RefugeeGroup RefugeeGroup { get; set; }

    public Guid RefugeeId { get; set; }
    public Refugee Refugee { get; set; }

	//Leader or head of Refugee group
    public bool IsDecisionMaker { get; set; }

	//This is the main contact to facilitate communications with the Refugee group
    public bool IsRefugeeGroupRepresentative { get; set; }

    public RefugeeGroupMembershipStatus Status { get; set; } // enum
    public string Details { get; set; } 
    
}
```