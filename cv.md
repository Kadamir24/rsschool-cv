# CV

## Amir Kaniyev

### Contact information
- email: amir.kaniyev@gmail.com
- github: [tab here to open my git](https://github.com/Kadamir24)


### Goal
I am an engineer who wants to upgrade his programmer skills as soon as possible

###Skills
- Golang
- HTML
- CSS
- R

###Code example

```go
func main() {
	args0 := os.Args[1:]

	f, err := os.Open("standard.txt")
	if err != nil {
		return
	}
	defer f.Close()

	var args string

	for _, word0 := range args0 {
		args = args + word0 + " "
	}

	words := strings.Split(args, "\\n")
	for _, word := range words {
		for i := 0; i < 8; i++ {
			for _, letter := range word {
				fmt.Print(ReadLine(f, 2+((int(letter)-32)*9)+i))
			}
			fmt.Println()
		}
	}
}

func ReadLine(f *os.File, n int) string {
	f.Seek(0, 0) //Устанавливает файловый указатель в определенную позицию
	bf := bufio.NewReader(f)
	var line string

	for lnum := 0; lnum < n; lnum++ {
		line, _ = bf.ReadString('\n')
		line = strings.TrimSuffix(line, "\n")

	}
	return line
}
```

###Education

i. **Kazakh-British Technical University. 2013-2017**
ii.**Alem school 2019-present**

###English
- B1 - Intermediate
