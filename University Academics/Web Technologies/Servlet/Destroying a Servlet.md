1. Allows active Threads to complete their service() method.
2. Container calls [[destroy()]] : Servlet releases resources (closing DB connections, freeing memory)
3. After `destory()` container releases all references to the [[Servlet]] instance, making it eligible for [[garbage collection]].