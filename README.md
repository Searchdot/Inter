```python
import hashlib

session_id = "187.250.219.226"
timestamp = "2023-11-8 12:48:08"
```

```python
hash_value = hashlib.sha256((session_id + timestamp).encode()).hexdigest()
tracker_code = hash_value[:8]

print("Tracker Code:", tracker_code)
```
