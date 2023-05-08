# Getting Started 

How to get up and running using Oloren Orchestrator.

## Installation

Installation instructions for Mac are [here](https://oloren-ai.notion.site/Orchestrator-Mac-OS-Install-Guide-a42271e138e24e6f855ece0ec3647067). 

## Adding Extensions

Under the extensions tab, add extensions by their name and docker image. This should take anywhere between a few minutes to an hour depending on how large the extension is.

Once added, make sure that in graph editor, using the add plug-in button (bottom left cloud icon), you also add the docker image there. 

Now, using the + button, you can search for add add nodes! 

Docker image for Basics extension:
| Name    | Public Image |
| :--------: | :-------: |
| Basics  | public.ecr.aws/d1r8e8k5/oloren-extension-olorenaiobasicsgitpub-new    |

## Node Functionality

Nodes are windows into what's going on under the hood. Press on a node, and you'll see the the following: 
1. A plus and minus sign at the top. For adding inputs. 
2. A plus and minus sign at the bottom. For adding outputs. 
3. A node ID on the right. 
4. A bunch of node metadata, super useful for debugging. 

Adding inputs and outputs is really important for networking together complex workflows. Nodes have two types of edges: black and blue.

Black edges are for passing around *values*. For example, if I have an add node with inputs of 1 and 2, connecting the black edge passes 3. 

Blue edges are for passing around *functions*. For the same add node, connecting the blue edge would pass around an add function with an available input node.


## Upload Files

Files can be uploaded via the "Upload Files" button at the top of graph editor. Files will be dropped in as a node, and those nodes can be then connected to other nodes as an input.

## Flow Functionality

Flows have tons of functionality. Beyond being run, they can be saved, shared, and loaded in to enable working across teams. If you ever need to look at the actual json or graph, they're viewable straight in graph editor too.

## Creativity

You're all set! Add more functionality by building extensions. We have a guide for that [here](https://oloren-ai.github.io/python-extension-lib/index.html).  Build complex workflows node by node. 