# [Null safety](https://dart.dev/null-safety)

- If you enable **null safety**, variables can’t contain null unless you say they can. 

- You can make a variable **nullable** by putting a **question mark (?)** at the end of its type. For example, a variable of type **int?** might be an integer, or it might be null. 

- If you know that an expression never evaluates to null but Dart disagrees, you can add **!** to assert that it isn’t null (and to throw an exception if it is). An example: **int x = nullableButNotNullInt!**

- **Uninitialized** variables that have a **nullable type** have an initial value of **null**. 

# Reference

- https://www.youtube.com/watch?v=iYhOU9AuaFs&list=PLjxrf2q8roU3wk7CDw4RfV3mEwOJbjx1k&index=10