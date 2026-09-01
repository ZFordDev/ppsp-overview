<div align="center">

# PPSP

### Peer-to-Peer Social Platform

**A social network where your devices are the network.**

</div>

## What is PPSP?

PPSP started with an idea proposed by the community:

**What if a social network didn't need the social network?**

Normally, you write a post and send it to a company's server. That server stores it, distributes it, and ultimately controls access to it.

PPSP takes the opposite approach.

Your posts live on **your device first**. Your friends' posts live on theirs. When your devices can reach each other, they sync directly.

No central server needs to hold the entire network together.

## How does that work?

When you create a post, it's stored locally and signed by your device.

When a friend comes online, your devices compare what they have and exchange what's missing.

But people aren't always online at the same time.

If Alice and Bob rarely overlap, but both know Charlie:

**Alice → Charlie → Bob**

Charlie can temporarily carry Alice's encrypted update and pass it to Bob later. Charlie doesn't need to read it - he's just carrying the package.

An optional home server, VPS, or hosted relay can do the same thing.

The important distinction is that **servers help the network; they aren't the network.**

## The basic idea

* **Local first** - Your device is the primary home of your data.
* **Peer-to-peer** - Friends exchange updates directly whenever possible.
* **Offline friendly** - Writing, reading, and managing your own data doesn't require a connection.
* **Encrypted relays** - Trusted nodes can carry updates without needing to read them.
* **Server optional** - Always-on relays improve availability without becoming a central authority.
* **Visible syncing** - PPSP should tell you what's actually happening instead of pretending everything instantly exists everywhere.

For example:

🔴 **Local** - Only on your device
🟡 **Propagating** - Moving through the network
🟢 **Synced** - Reached the known network

The exact meaning of "synced" is still being explored as the protocol develops.

## Project structure

PPSP is being designed as a small ecosystem rather than one giant application.

| Repository          | Purpose                                                             |
| :------------------ | :------------------------------------------------------------------ |
| **`ppsp-overview`** | Architecture, protocol decisions, schemas, and project coordination |
| **`ppsp-core`**     | Local storage, sync engine, events, and P2P networking              |
| **`ppsp-desktop`**  | Desktop client                                                      |
| **`ppsp-server`**   | Optional store-and-forward relay                                    |
| **`ppsp-mobile`**   | Mobile client                                                       |

The technology behind these components isn't locked in yet. PPSP is still an experiment, and the architecture should decide the tools rather than the other way around.

## A community idea

PPSP wasn't originally sitting on a roadmap waiting to be built. The idea came from the community and grew into something interesting enough to explore properly.

That's worth acknowledging.

Projects like PPSP - and previously Glint - are a reminder of why community ideas matter. Someone suggesting an idea I hadn't considered can challenge what I think I can build and push a project in directions I wouldn't have reached alone.

So, **thank you to the community for proposing PPSP and continuing to throw interesting problems my way.**

Great projects don't always start with a roadmap. Sometimes they start with someone asking:

**"Could you build this?"**

## Contributing

PPSP is very early, and that's the best time to challenge it.

Question the architecture. Find the edge cases. Suggest something better. Build an experiment.

If you're interested in local-first software, P2P networking, distributed systems, or decentralized social software, you're welcome to get involved.

**The protocol matters more than any one implementation.**

