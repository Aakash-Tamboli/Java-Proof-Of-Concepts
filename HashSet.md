So HashSet Or Set Internally used Map or hashMap proof of concepts:
Video https://youtu.be/7k0VYHuUF6g


## What is Set?
Set is interface where HashSet,TreeSet,LinkedHashSet impliments Set interface.

## When We Use HashSet,TreeSet,LinkedHashSet
If We want performace is our fast priority and in traversal order not matter then HashSet is Best.
If We Want that we will compromise with little performance but in traversal data will come into sorted order then TreeSet is Best.
If We Want that want that in traversal data will come into order of how we added into set then go with LinkedHashSet but It is slow compare to other's set Option.

Demo Code:
```
java

import java.util.*;
class psp
{
public static void main(String[] args)
{
Set<String> setForHashSet,setForTreeSet,setForLinkedHashSet;
setForHashSet=new HashSet<>();
setForTreeSet=new TreeSet<>();
setForLinkedHashSet=new LinkedHashSet<>();

setForHashSet.add("Ujjain");
setForTreeSet.add("Ujjain");
setForLinkedHashSet.add("Ujjain");

setForHashSet.add("dewas");
setForTreeSet.add("dewas");
setForLinkedHashSet.add("dewas");

setForHashSet.add("Goa");
setForTreeSet.add("Goa");
setForLinkedHashSet.add("Goa");

setForHashSet.add("Delhi");
setForTreeSet.add("Delhi");
setForLinkedHashSet.add("Delhi");

setForHashSet.add("Indore");
setForTreeSet.add("Indore");
setForLinkedHashSet.add("Indore");

setForHashSet.add("Mhow");
setForTreeSet.add("Mhow");
setForLinkedHashSet.add("Mhow");

setForHashSet.add("Mumbai");
setForTreeSet.add("Mumbai");
setForLinkedHashSet.add("Mumbai");

setForHashSet.add("Pune");
setForTreeSet.add("Pune");
setForLinkedHashSet.add("Pune");

System.out.println("Traversal Of HashSet where Speed is Fast but data will come into random order");
setForHashSet.forEach((data)->{
System.out.println(data);
});

System.out.println("Traversal Of TreeSet where speed little bit slow but data will come into sorted order");
setForTreeSet.forEach((data)->{
System.out.println(data);
});

System.out.println("Traversal Of LinkedHashSet where speed super slow compare to other's two's but data will come in order to how we added into set");
setForLinkedHashSet.forEach((data)->{
System.out.println(data);
});


}
}

```