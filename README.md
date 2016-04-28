# graph-traverse

Learning graph traversal implementations from http://hueypetersen.com/posts/2013/06/25/graph-traversal-with-clojure/

Also played with the fn interfaces a bit


I recommend checking out https://github.com/Engelberg/ubergraph if this interests you.

## Usage

All the functions are in core. No tests written

EX.
```
(traverse (get-graph) {:direction :depth
                       :start :1})
=> (:1 :3 :4 :5 :6 :2 :7 :8 :9 :10 :11 :12 :13)

(traverse (get-graph) {:direction :breadth
                       :start :1})
=> (:1 :2 :3 :4 :7 :5 :8 :6 :9 :10 :11 :12 :13)

(traverse (get-graph) {:direction :breadth
                       :start :13})
=> (:13 :4 :2 :3 :5 :7 :1 :6 :8 :9 :10 :11 :12)
```

## License

Copyleft, do whatever but please be good.
