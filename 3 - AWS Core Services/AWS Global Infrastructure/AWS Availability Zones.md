# Availability Zones (AZs)

* **AWS Availability Zones** (AZs) are a collection of data centers in a specific **AWS Region**
* Each Availability Zone is **physically isolated from the other, but are connected by a fast, low latency network**
* Each Availability Zone is a **physically distinct, independent infrastructure, that is physically and logically separate**
* Availability zones have an **uninterruptible power supply**, **on - site backup generators**, **cooling equipment**, **network connectivity**, and are **supplied by different grids from indepedent utility companies for power**
* Availability Zones are networked through multiple Tier 1 transit providers
* Because Availability Zones are isolated, *they are protected from failures in other Availability Zones*
* This ensures *high availability and data redundancy within a region*
* If one Availability Zone goes down, another can handle requests
* AWS recommends as a best practice to provision data across multiple Availability Zones
