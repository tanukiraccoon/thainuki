# Thainuki

Thainuki is a Python package inspired by the clever adaptability of the mythical Tanuki, combining the art of linguistic transformation.

ไทยนูกิ สร้างภาษาเฉพาะจากภาษาไทย

Supported Languages:
-  Lu language (ภาษาลู)
-  Malagor language (ภาษามะละกอ)
  
Other Tool:
- Thai spoonerism (คำผวน)

## Usage

### Installation

You can install Thainuki using pip:

```shell
pip install thainuki
```

### Example Usage

Here's an example of how to use the Thainuki package and call its functions:

```python
from thainuki import malagor, thai2lu, lu2thai, khamphuan

# Lu language generator
thai2lu("ไทยนูกิ") # => Output: ['ลัยทุย','ลานู','หลิกุ']

# Reverse Lu language
lu2thai("ลัยทุย ลานู หลิกุ") # => Output: ['ทัยนูกิ']

# Malagor language generator
malagor("ไทยนูกิ") # => Output: ['ทะละกัย','นะละกู','กะละกิ']

# Thai spoonerism
khamphuan("ไทยนูกิ") # => Output: ['ทินูกัย','ถินูกัย','ทัยนิกู่','ทัยหนิกู']
```
## Limitation
- If the Thai tone is falling tone (too/โท) and the original word uses a high-class letter, this script will use a low-class letter for spelling. Please keep this in mind when using the generator.
- When spelling the vowel sounds represented by the characters "ไ-" and "ใ-", the generator will use the characters "-ัย" instead.
