```cs
class RefugeeDocument
{
	public Guid DocumentId { get; set; }
	public Document Document { get; set; }

	public Guid RefugeeId { get; set; }
	public Refugee Refugee { get; set; }

	public RefugeeDocumentStatus Status { get; set; }

}
```