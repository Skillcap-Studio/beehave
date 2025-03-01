# Composite Nodes

Composite nodes are essential components of Behavior Trees, allowing you to create logic flows by combining conditions and actions. A composite node is a parent node that executes its children in a specific order, helping to define complex behaviors for your game characters or objects.

## How do they work?
Composite nodes enable you to compose your Behavior Tree by connecting various nodes together. They serve as a glue between leaf nodes (conditions and actions) and facilitate decision-making processes within the tree. By connecting leaf nodes to composite nodes, you can create a hierarchy that represents your desired game logic.

## Building Your Behavior Tree
To create a Behavior Tree, you'll need to link various nodes together, with composite nodes serving as the foundation for your tree's structure. Here's a general outline of how to build a Behavior Tree using composite nodes:

1. Start by defining conditions and actions as leaf nodes.
2. Use composite nodes to create a hierarchical structure that connects these leaf nodes.
3. Connect composite nodes to each other as needed to define the overall logic of your Behavior Tree.

Keep in mind that the specific types of composite nodes you use, such as Selectors or Sequences, will depend on the desired behavior and logic flow you want to achieve. By combining these nodes, you can create intricate AI behavior that is modular, reusable, and easy to manage.

With composite nodes, you can craft unique and dynamic Behavior Trees for your game characters and objects, giving them the ability to make decisions and interact with the game world in a more engaging and lifelike manner.

## Restarting a composite

If a parent node restarts a child node, it means that the parent node will start the child node from scratch the next time it is ticked. This means that any progress made by the child node will be reset, and it will start its execution from the beginning.

## Ticking again a composite

If a parent node ticks a child node again, it means that the parent node will immediately tick the child node again on the next frame, without waiting for the current frame to finish executing. This allows the child node to continue its execution from where it left off without resetting its progress.

In other words, restarting a child node means that the parent node will give the child node a fresh start, while ticking it again means that the parent node will let the child node continue its execution from where it left off.
