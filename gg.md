```graphviz
digraph self_locking_mechanisms {
    rankdir=LR;
    node [shape=ellipse, style=filled, color=lightblue, fontname="Arial", fontsize=12];

    "金融自锁" -> "政策自锁" [label="金融机构的过度放贷为地方政府的土地财政提供资金", fontsize=10, fontname="Arial"];
    "政策自锁" -> "行为自锁" [label="维持高房价的政策增强市场参与者对房价上涨的预期", fontsize=10, fontname="Arial"];
    "行为自锁" -> "金融自锁" [label="市场参与者的过度投机推动金融机构的扩张", fontsize=10, fontname="Arial"];
    "行为自锁" -> "政策自锁" [label="市场参与者的过度投机巩固地方政府对土地财政的依赖", fontsize=10, fontname="Arial"];

    // 添加节点标签
    "金融自锁" [label="金融自锁\n(金融机构的过度放贷)", fontsize=12, fontname="Arial"];
    "政策自锁" [label="政策自锁\n(维持高房价的政策)", fontsize=12, fontname="Arial"];
    "行为自锁" [label="行为自锁\n(市场参与者的过度投机)", fontsize=12, fontname="Arial"];
}