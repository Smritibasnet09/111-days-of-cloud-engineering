# Amazon S3 – Advanced Concepts Notes

---

## S3 Lifecycle Rules

### What it is

Automates the movement and deletion of S3 objects over time using defined rules.

### Why use it

* Reduce storage cost by moving data to cheaper storage classes
* Automatically manage and clean up old or unused data

### Actions

**Transition**

* Moves objects from one storage class to another based on age
  (e.g., Standard → Standard-IA → Glacier for long-term storage)

**Expiration**

* Permanently deletes objects after a specified number of days

### Scope

Rules can apply to:

* Entire bucket
* Specific objects using filters:

  * Prefix (e.g., `images/*` → only applies to image folder)
  * Tags (e.g., `Department: Production` → only tagged objects)

### Quick Memory

Lifecycle = Automatically move or delete data based on time rules

---

## S3 Analytics – Storage Class Analysis

### What it is

Analyzes how frequently objects are accessed to suggest better storage classes.

### Key Points

* Works for:

  * Standard (frequently accessed data)
  * Standard-IA (infrequently accessed data)
* Not supported:

  * One-Zone IA
  * Glacier classes

### Timing

* Takes 24–48 hours after enabling to start showing data
* Reports are updated daily with new insights

### Use Case

* Helps decide when to transition data using Lifecycle Rules

### Quick Memory

Analytics = Helps decide the right time to move data to cheaper storage

---

## S3 – Requester Pays

### Default

* Bucket owner pays for:

  * Storage
  * Data transfer and requests

### With Requester Pays

* The person accessing the data pays for:

  * API requests
  * Data download charges

### Requirements

* Must use authenticated AWS account
* Anonymous (public) access is not allowed

### Use Case

* Useful when sharing large datasets with others without paying for their usage

### Quick Memory

Requester Pays = The user accessing the data is responsible for the cost

---

## S3 Event Notifications

### What it is

Sends notifications when specific events happen in an S3 bucket.

### Supported Events

* ObjectCreated (file uploaded)
* ObjectRemoved (file deleted)
* ObjectRestore (restored from archive)
* Replication (data copied across regions)

### Filtering

* Can filter events based on object name patterns
  (e.g., `*.jpg` → only image files)

### Features

* Supports multiple notification configurations per bucket
* Events are delivered almost in real-time (usually seconds)

### Use Case

* Automatically trigger processing tasks (e.g., generate thumbnails after upload)

### Quick Memory

Event Notification = Event happens → automatic action is triggered

---

## S3 + Amazon EventBridge

### What it is

An advanced event routing service that captures and processes S3 events with more flexibility.

### Capabilities

* Advanced filtering using JSON-based rules
* Can filter by object metadata, size, and name patterns

### Destinations

* Step Functions (workflow automation)
* Kinesis Streams (real-time data streaming)
* Firehose (data delivery service)

### Features

* Event archiving for storing past events
* Event replay to reprocess previous events
* Reliable and scalable event delivery system

### Use Case

* Build complex, event-driven architectures reacting to S3 changes

### Quick Memory

EventBridge = Advanced event filtering and routing system for scalable application.

---

## Final Revision Summary

| Feature            | Main Idea                                    |
| ------------------ | -------------------------------------------- |
| Lifecycle          | Automate movement and deletion of data       |
| Analytics          | Recommend cost-efficient storage transitions |
| Requester Pays     | Shift data access cost to the requester      |
| Event Notification | Trigger actions when S3 events occur         |
| EventBridge        | Advanced event routing and processing system |

---
