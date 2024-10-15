## How-To Guide: Preparing Your Environment for the Latest Build

This guide will walk you through the essential steps to prepare your environment for the latest build, ensuring smooth deployment and functionality.

Overview: Checkout → clear cache → migrate → sync → Done

---

### 1. **Check Out the Most Recent Build**

Before starting any updates, ensure you're working with the most up-to-date codebase:

- **Command**: `git checkout "build"` (or your specific branch)
- **Pull Latest Changes**: `git pull "build"`

This ensures you're working with the latest changes and bug fixes from your team.

### 2. **Clear Cache**

Caching can cause issues when deploying new builds, as it may store outdated or irrelevant data. Clearing the cache helps to ensure no conflicting data persists:

- **Run the Cache Clear Script**: Execute the clear cache script to reset cached data
```bash
./scripts/clear_cache.sh
```

### 3. **Run Database Migrations**

Migrations update your database schema in line with any changes made in the codebase, such as adding new tables, modifying columns, or adjusting relationships:

- **Command**:
```bash
./scripts/migrate
```

This script ensures your database schema matches the latest version of the application code.

Note_: Always check the migration logs to ensure no errors occur during this step.
### 4. **Sync Data**

If your application requires syncing certain data after migrations (such as updating static data or syncing with external services), this step ensures everything is in place:

- **Run the Sync Script**: This step synchronizes essential data to ensure consistency and functionality with the updated build.