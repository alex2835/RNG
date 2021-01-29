###### RNG

```c++

RNG random;

for (int i = 0; i < 100; i++)
{
  printf("%f \n", random.Get<float>(-10, 10));
}

template <typename T>
T Get(const T& min_value = std::numeric_limits<T>::min(),
      const T& max_value = std::numeric_limits<T>::max());
```

