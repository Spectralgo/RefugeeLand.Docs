# AdditionalFamilyMemberMemberShip

```cs
class AdditionalFamilyMemberFamilyMembership
{
    public Guid FamilyId { get; set; }
    public Family Family { get; set; }

    public Guid AdditionalFamilyMemberId { get; set; }
    public AdditionalFamilyMember AdditionalFamilyMember { get; set; }

	//Leader or head of family
    public bool IsDecisionMaker { get; set; }

	//This is the main contact to facilitate communications with a family
    public bool IsFamilyRepresentative { get; set; }

    public RefugeeFamilyMemberStatus Status { get; set; } // enum
    public string Details { get; set; } 
}
```

## Description
This class is an hybrid relational model. It describes the current status and role of a family members, who is neither a refugee or host, relative to a paricular family.

[Hybrid Relational Model](https://docs.refugee.land/v/the-standard-faq/the-standard-wiki/0-introduction/0.0-purposing-modeling-and-simulation?q=hybrid+models):
