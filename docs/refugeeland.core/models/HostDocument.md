```cs
class HostDocument
{
	public Guid DocumentId { get; set; }
	public Document Document { get; set; }

	public Guid HostId { get; set; }
	public Host Host { get; set; }

	public HostDocumentStatus Status { get; set; }

}
```