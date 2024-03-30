moved to [https://github.com/molikto/blog/discussions/1]


struct TreeItem<K, T, tree: Tree<K, T>> {
  parent: ]tree.nodes[
  fi: Float // fractional indexing
  data: T
}

struct Tree<K, T> { tree -> 
  nodes: Map<K, TreeItem<K, T, tree>>
}


type IntTree = Tree<UUID, Int>

type FloatTree = Tree<UUID, Float>

struct Database {
  ints: IntTree
  floats: FloatTree
}
