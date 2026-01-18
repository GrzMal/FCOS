# Instructions for verifying computational results

These steps explain how to reproduce the computations from the article:

**“Construction of free curves by adding osculating conics to a given cubic curve.”**

---

## 1. Modify SINGULAR to allow field extension computations

You can do this in two ways:

### **Option A — Replace the original library file**

1. Download the following files:
   - `classify.txt`
   - `cmp.txt`

2. Rename the file `classify.txt` to **`classify.lib`**.

3. Replace the original file `classify.lib` located in:

(...\cygwin64\usr\local\share\singular\LIB)


(or the equivalent SINGULAR library path on your system).

---

### **Option B — Modify the library only for the current session**

1. Download the following files:
- `classify.txt`
- `cmp.txt`

2. Open the file **`cmp.txt`** and add the following line **after line 49**:

```singular```
`<"classify.txt";`

3. Save the file.

4. In SINGULAR, run the modified `cmp.txt` file:

## Reference

If you use this code in your work, please cite the following paper:

A. Dimca, G. Ilardi, G. Malara, P. Pokora
*Construction of free curves by adding osculating conics to a given cubic curve*
