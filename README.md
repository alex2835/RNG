###### RNG

C++ 20

```c++

RNG random;
for (int i = 0; i < 10; i++)
{
		printf("int    - %d \n", random.Get<int>(-10, 10));
		printf("uint   - %u \n", random.Get<uint32_t>(0, 10));
		printf("float  - %f \n", random.Get<float>(-10, 10));
		printf("double - %lf\n", random.Get<double>(-10, 10));
		printf("\n");
}

template <typename T>
T Get(const T& min_value = std::numeric_limits<T>::min(),
      const T& max_value = std::numeric_limits<T>::max());
```

