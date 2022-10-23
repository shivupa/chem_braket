# chem-braket.sty
## Macros for chemist's bra-ket (|) notation
## Shiv Upadhyay     shivnupadhyay@gmail.com     Last modified 06-Oct-2022.
This is free, unencumbered, unsupported software.

Commands defined are (similar to original with c for chemists):
```
\cbra{ }   \cket{ }   \cbraket{ }   (small versions)
\Cbra{ }   \Cket{ }   \Cbraket{ }   (expanding versions)
```

The "small versions" use fixed-size brackets independent of their
contents, whereas the "expanding versions" make the brackets and 
vertical lines expand to envelop their contents (internally using 
the \left and \right commands).  You should use the vertical bar
character "|" to input any extra vertical lines.  In \Braket these
vertical lines will expand to match the arguments. E.g.,
```
  \Braket{ \phi | \frac{\partial^2}{\partial t^2} | \psi }
```


The original implementation had this note:
> Because each definition is so small, it makes no sense to have a 
> complicated generic version for many bracket styles.  Instead, 
> you can just copy the definitions and change \langle or \rangle,
> to what you like.

This unfortunately led to the existence of this package.
