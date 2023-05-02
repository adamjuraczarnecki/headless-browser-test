# headless-browser-test

based on [Louis Klimek article](https://piprogramming.org/articles/6-Ways-to-detect-a-headless-Browser-with-JavaScript--How-to-detect-a-Headless-Browser-0000000030.html)

```python
def test():
    driver.get('https://adamczarnecki.github.io/headless-browser-test/')
    tests = driver.find_elements(By.CSS_SELECTOR, 'tbody tr')
    for test in tests:
        name, result = test.find_elements(By.TAG_NAME, 'td')
        print(f'{name.text:<25}: {result.text}')
```
