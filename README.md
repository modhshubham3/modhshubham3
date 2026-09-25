## Shubham Modh

Full-stack .NET developer in Ahmedabad, India. I build and run real-time systems —
the kind where being wrong is visible on a control-room screen within ten seconds.

### What I work on

I'm the primary developer on **AVLS**, a GPS fleet-tracking platform used by three
government transport authorities. The largest deployment live-tracks around **700
buses**, each reporting a position every ~10 seconds — roughly **6 million packets a
day**.

Devices send raw TCP → a .NET service frames and parses vendor protocols → Kafka →
a 32-worker consumer pool enriches each position against Redis → history lands in
partitioned PostgreSQL tables while Tile38 answers the geofence questions →
ASP.NET Core APIs and SignalR push it to an Angular control room.

Things I built inside it: the live tracking map, trip management, geofence-based
stop-arrival detection, ETA computation, an emergency panic-alert system, 50+
operational reports, and a booking/refund module.

### Stack

**Backend** C# · ASP.NET Core · Web API · ADO.NET / stored procedures
**Frontend** Angular · TypeScript
**Data** PostgreSQL (partitioning, query tuning, logical replication) · Redis
**Streaming & real-time** Apache Kafka · SignalR · Tile38
**Infra** GCP (Compute Engine, VPC) · Docker · Linux

### Where else to find me

| | |
|---|---|
| Portfolio | [shubham-modh.vercel.app](https://shubham-modh.vercel.app) |
| Freelance | [shubham-builds-eight.vercel.app](https://shubham-builds-eight.vercel.app) |
| LinkedIn | [shubham-modh](https://www.linkedin.com/in/shubham-modh-26a23021b) |
| Email | modhshubham3@gmail.com |

> Most of my production work sits in private government repositories, so the code
> here is limited to what I can show publicly — both portfolio sites are built and
> deployed from this account.
