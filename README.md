### README.md

# Kadane Advanced Library

A Python library implementing Kadane's Algorithm and its advanced variations:
- Basic Kadane (Max subarray sum)
- Max subarray with result
- Min length subarray constraint
- 2D max submatrix finder
- Subarray visualizer

## 🔄 General Use
This library is designed for **any user**, **any data**, and **any use case** involving:
- Time series
- Mood trackers
- Sensor data
- Scores/stats
- Matrices or grids

---

## 📦 Installation
```bash
pip install kadane-adv
```

## 🚀 Usage
```python
from kadane_advanced import kadane_max_sum, kadane_max_subarray, kadane_with_min_length, kadane_2d, visualize_subarray

# Example 1: 1D array
arr = [-2, 1, -3, 4, -1, 2, 1, -5, 4]
print("Max Sum:", kadane_max_sum(arr))

max_sum, subarray = kadane_max_subarray(arr)
print("Max Subarray:", subarray)
visualize_subarray(arr, subarray)

# Example 2: 2D array
matrix = [
    [1, 2, -1],
    [-3, 4, 5],
    [2, -6, 3]
]
max_sum, top_left, bottom_right = kadane_2d(matrix)
print("2D Max Sum:", max_sum)
print("Coordinates:", top_left, bottom_right)
```

## 🧪 Testing
```bash
pytest tests/
```

## 🧭 Learning Path (Inspired by Product School)
1. **Understand the Problem**: Learn subarray and time-series sum problems.
2. **Implement Basic Kadane**: Learn max sum logic using positive/negative balance.
3. **Add Constraints**: Try with min-length or fixed-length subarrays.
4. **Work on 2D Extension**: Extend to matrix/grid-based applications.
5. **Use Visualization**: To debug or present subarray results in real-time.
6. **Deploy or Wrap**: Turn into CLI, web API, or integrate into dashboards.

## 📄 License
MIT
