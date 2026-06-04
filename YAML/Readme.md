# 📚 YAML Learning Repository

A comprehensive guide documenting my journey of learning **YAML (YAML Ain't Markup Language)** - a human-readable data serialization language widely used in DevOps, configuration management, and cloud-native applications.

## 🎯 About YAML

YAML is a lightweight, easy-to-read data format that emphasizes human readability while remaining machine-parseable. It's extensively used in:

- **DevOps Tools**: Docker Compose, Kubernetes, Ansible, Jenkins
- **Configuration Files**: Application configs, CI/CD pipelines
- **Data Exchange**: Alternative to JSON and XML
- **Infrastructure as Code (IaC)**: Cloud infrastructure definitions

### Key Characteristics

✅ **Human-Readable**: Uses indentation and simple syntax  
✅ **Minimal Syntax**: Less cluttered than JSON/XML  
✅ **Type-Aware**: Supports strings, integers, floats, booleans, lists, and dictionaries  
✅ **Language-Agnostic**: Can be parsed in any programming language  

---

## 📁 Repository Structure

This repository contains practical examples organized by complexity level:

### **1. Basic Fundamentals** (`hello.yml`)
Covers the essentials of YAML syntax:

```yaml
# Key-value pairs
Name: Divya
job: Devops

# Lists (Block Style)
cities:
  - Mumbai
  - Delhi
  - Kolkata

# Lists (Flow Style)
cities: [New Delhi, Mumbai]

# Inline Dictionary
{fruit: mango, age: 60}
```

**Topics Covered:**
- Key-value pairs
- String, integer, and dictionary data types
- List representations (block and flow style)
- Document separators (`---`) and terminators (`...`)
- YAML is case-sensitive
- Importance of indentation/spacing

### **2. Data Types** (`keyDatatypes.yml`)
Exploring different data types and format options:

```yaml
# String Variables
name: Divya
fruit: "Mango"
job: 'Devops'

# Multi-line Strings
bio: |
  Hey my name is Divya.
  I am a very nice person.

# Folded Strings (single line)
message: >
  This will
  all be
  in one single line

# Numeric Types
number: 89          # Integer
marks: 45.67        # Float

# Boolean Values
isActive: true      # or: yes, y, Y
isCompleted: false  # or: no, n, N, False

# Type Casting
zero: !!int 0
positiveNum: !!int 45
negativeNum: !!int -56
binaryNum: !!int 0b11001
octalNum: !!int 0o6574
```

**Topics Covered:**
- String data types and quoting
- Literal block (`|`) vs folded (`>`) syntax
- Numeric types (int, float, binary, octal)
- Boolean values and their variations
- Type casting with `!!` prefix

### **3. Advanced Data Structures** (`AdvanceDatatypes.yml`)
Working with complex nested data:

```yaml
# Sequences
student: !!seq
  - marks
  - name
  - roll_no

# Sparse Sequences (with empty elements)
sparse_seq:
  - how
  - hey
  -      # Empty element
  - sup

# Nested Sequences
- [mango, apple, banana]
- [rose, lily, sunflower]
- [red, pink, white]
```

**Topics Covered:**
- Explicit sequence declaration
- Sparse sequences with empty values
- Nested lists and complex hierarchies
- Sequence vs mapping structures

### **4. Other Examples**
- `school.yml` / `school.json` / `school.xml` - Format comparisons
- `YAMLdevopstools.md` - YAML usage in DevOps tools

---

## 🛠️ Key Concepts Mastered

| Concept | Description |
|---------|-------------|
| **Indentation** | 2 or 4 spaces define hierarchy (not tabs) |
| **Lists** | `- item` syntax or flow style `[item1, item2]` |
| **Dictionaries** | Key-value pairs with `key: value` format |
| **Strings** | Can be quoted or unquoted; support multi-line |
| **Data Types** | Strings, integers, floats, booleans, null, dates |
| **Anchors & Aliases** | `&anchor` to reference and `*anchor` to reuse |
| **Comments** | `#` for single-line comments |
| **Document Markers** | `---` separates documents; `...` ends document |

---

## 💡 Real-World Applications

### Docker Compose Example
```yaml
version: '3'
services:
  web:
    image: nginx:latest
    ports:
      - "80:80"
  db:
    image: postgres:13
    environment:
      POSTGRES_PASSWORD: secret
```

### Kubernetes Example
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-pod
spec:
  containers:
  - name: app
    image: my-app:latest
```

### Ansible Playbook Example
```yaml
---
- hosts: all
  tasks:
    - name: Install packages
      apt:
        name: git
        state: present
```

---

## 📖 Learning Resources

- **Official YAML Specification**: [yaml.org](https://yaml.org)
- **Practice Scenarios**: Docker, Kubernetes, CI/CD pipelines
- **Validation**: Use online YAML validators (yamllint, YAML online parsers)

---

## 🚀 Next Steps

- Explore YAML in **Kubernetes** manifests
- Master **Ansible** for infrastructure automation
- Learn **GitOps** workflows with YAML-based IaC
- Implement configuration management with YAML

---

## 📝 Notes

> YAML is incredibly valuable in modern DevOps culture. Understanding YAML syntax deeply will significantly enhance your ability to work with popular DevOps tools and cloud platforms.

---

**Happy Learning!** 🎓
