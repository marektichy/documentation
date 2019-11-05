# Depth

**When sending a transaction to a node, you can specify a depth variable. The depth defines how many milestones in the past a [node](../basics/nodes.md) starts the [tip selection algorithm](../basics/the-tangle.md#tip-selection). The greater the depth, the farther back in the [Tangle](../basics/the-tangle.md) the node starts. A greater depth increases the time that nodes take to complete tip selection, making them use more computational power.**

## Advice for choosing a depth

When choosing a depth, you should consider the following question.

### What is the maximum depth that your node will allow?

To restrict the depth, nodes can define a maximum value for it in the [`MAX-DEPTH`](root://node-software/0.1/iri/references/iri-configuration-options.md#max-depth) configuration option.

If you aren't connected to your own node, you should consider doing so. This way, you can make sure that you're using a valid depth.

If you want to use a third-party node, you can check the value of this configuration option by calling the [`getNodeAPIConfiguration` endpoint](root://node-software/0.1/iri/references/api-reference.md#getnodeapiconfiguration).