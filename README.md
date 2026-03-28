```go
type Louis struct {
      Name              string
      Email             string
      LinkedIn          string
      TimeZone          string
      QuoteOfTheDay     string
      FavoriteLanguages []string
      Hobbies           []string
}

func NewLouis() Louis {
      return Louis{
              Name:          "Louis Kauer",
              Email:         "louis.kauer@proton.me",
              LinkedIn:      "linkedin.com/in/louis-kauer",
              TimeZone:      "CEST",
              QuoteOfTheDay: "The future of software is in orchestration, not just code. - Kelsey Hightower",
              FavoriteLanguages: []string{"Go", "C++", "Rust", "Kotlin"},
              Hobbies:           []string{"Hiking", "Running", "Cycling", "Playing the piano"},
      }
}

func (l Louis) StartDay() {
      for l.IsAwake() {
              l.Code()
      }
}
```
