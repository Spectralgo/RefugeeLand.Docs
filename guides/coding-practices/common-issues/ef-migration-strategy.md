---
description: >-
  If you are working within a team, it is really important to have a process
  setup to prevent migration conflicts.
---

# EF Migration Strategy



## Process to prevent conflict

1. You are about to submit a pull request with a database migration inside.
2. Pull latest from the target branch `origin main` in our case.
3. Resolve any conflicts if needed.
4. If there's any pending migrations coming from the remote branch, make sure you delete your branch and recreate it.
5. <mark style="color:red;">**Shout out !!!**</mark> Tell everyone in the team saying that this pull request has a migration inside. Either using Discord or any other effective mean.

{% hint style="warning" %}
* Make sure that you didn't just merge the last migration to your branch
* Make sure you built your migration UPON the last one.
* If anyone is about to submit a pull request with a database migration, he/she will wait until the pull request is completed.
{% endhint %}

{% embed url="https://docs.microsoft.com/en-us/ef/core/cli/dotnet" %}
For dotnet CLI
{% endembed %}

{% embed url="https://docs.microsoft.com/en-us/ef/core/cli/powershell" %}
&#x20;For Visual Studio
{% endembed %}

### Stack Overflow
[How to unapply a migration in asp net core with EF Core](https://stackoverflow.com/questions/38192450/how-to-unapply-a-migration-in-asp-net-core-with-ef-core)

### MS Docs

[Migrations in Team Environments](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/teams)

[Migrations Overview](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/?tabs=dotnet-core-cli)&#x20;

[Applying Migrations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/applying?tabs=dotnet-core-cli)

[Managing Migrations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations/managing?tabs=dotnet-core-cli)

[Entity Framework Core tools reference](https://docs.microsoft.com/en-us/ef/core/cli/)

### Blog posts about this

https://passos.com.au/overcoming-ef-core-migration-conflicts/ https://jkdev.me/handling-ef-core-migrations/

### Resolving EF Migrations conflicts

Might be obvious, but just to mention here:

Remove migrations up to the point of the conflict: dotnet ef migrations remove.

If the EF commands are not working to rollback because of the conflict, you can: 1. Copy the content of the BuildTargetModel method inside the \*.Designer.cs file from the migration you want to rollback. 2. Replace the whole content of the BuildModel method in the \*ContextSnapshot. 3. Create a new migration dotnet ef migrations add \[NAME OF MIGRATION]

#### What did we learn?

We learn from challenges and although this was a quite painful one, we did learn a few things.

* The Migrations/\*.Designer.cs files are used in design time only (I know it's obvious). And they're really only used when you want to roll back a migration dotnet ef migrations remove.
* You can remove all Migrations/\*.Designer.cs if you want to and it's not going to impact any future migrations, but if you try to remove a migration, it will jump to the last \*.Desiner.cs file it can find. For example, we tried removing the 2 last \*.Designer.cs files and when running dotnet ef migrations remove, it actually removed the 3rd last migration.
* Breaking the migration stream doesn't really affect anything when applying migrations.
* EF does NOT use the Migrations/\*.Designer.cs files to apply migrations.

### YouTube Migrations Tutorials

https://youtu.be/YUmSwR6jjlU?t=55

### Unapply migration (if your database  was already updated)
```shell
//step 1 reverting last migartion
dotnet ef database update <previous-good-migration>


//step 2 remove migration files by hand, there is no command, keep the snapshot file.

//step 3 remove the last migration from the snapshot
dotnet ef migrations remove 

```