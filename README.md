
# Hey, I'm Rafael!

So this is my brief apresentation, hope you like it! There's some topics and interesting easter eggs scattered throughout the code 👨🏽‍💻

🇧🇷/🇺🇸
```go




package main 
import (
	"fmt"
	"math/rand"
	"time"
)
type TheVoid struct {
	Name string
	age any
	Aboutme []string
}
func ThisIsMe(){
	whoami := TheVoid{
		Name: "Rafael",
		Aboutme: []string{"Beginner programmer", 
		"Music enjoyer", 
		"Spotify", 
		"Coding", 
		"Portuguese/English", 
		"Brazilian Student",
	},
	}
	fmt.Println(whoami.Name)
	for i, value := range whoami.Aboutme{
		fmt.Printf("%d. %s\n",i+1, value )
	}
}
func Interests() (map[string]string){
	return map[string]string{
		"Programming":"Building projects and Programming is my weirdest hobby.",
		"Golang":"I started learning some weeks ago. I dont have genius thoughts yet.",
		"Games":"I love playing games and chill a bit sometimes",
		"Goal":"I'd love to contribute with Go communnity since it's so cool to be a part of.",
	}
}
type Song struct {
	Artist string 
	Genre string 
	Obs	[]string
}
func MusicTaste() []Song {
	return []Song{
		{Artist: "Mitski", 
		Genre: "Indie/Alt/Pop", 
		Obs: []string{"Since she's my taste pioneer, It'd be rude of me if she wouldn't have a place here"},
	},
		{Artist: "Linkin Park", 
		Genre: "Nu Metal/Recently Pop-mixed (I guess?)", 
		Obs: []string{"They've played such an important role during rough times. Never forgetting them at all"},
	},
		{Artist: "Fiona Apple", 
		Genre: "Alternative/Art-pop", 
		Obs: []string{"Recently added to my taste, but it makes her unique. I don't have much to say tho. She just fits it well"},
	},
		{Artist: "Beabadoobee", 
		Genre: "Mostly subgenres of Rock/Folk-pop/Bedroom pop/Samba", 
		Obs: []string{"Same as Fiona but I have known her music for a bit longer"},
	},
		{Artist: "Limp Bizkit", 
		Genre: "Nu Metal", 
		Obs: []string{"Nothing to say.. Same, it fits well too"},
		}, 
		{Artist: "Rammstein", 
		Genre: "Industrial Metal and some other shit I dunno", 
		Obs: []string{"Yeah. It's listenable. I have no great things to say, but they're a respected band."},
	},
		{Obs: []string{"I also listen to stuff like MPB (Música Popular Brasileira) and some specific genres, but it'd make this list even longer"}},
	}
}
const (
	Studying = "High School/Learning Go structures"
	Gaming = "Chill time!🎮"
	Coding = "Building something Cool"
)
func CurrentStats() string {
	status := Studying 
	return status 
}

func SkillLevel_Goal(hours int16)string{
	if hours < 100 {
		return "Novice (Learning the Basics)"
	} else if hours < 500 {
		return "Apprentice (Building projects)"
	} 
	return "Mage (Writing Entire Buildings)"
	//   < 100, I'm a novice! :))
} 

type Setup struct {
	OS string 
	Editor []string 
	Theme string
}
func SetupSpec() Setup {
	sys := Setup{
		OS: "Linux-Manjaro",
		Editor: []string {"VScode", "Considering NeoVim"},
		Theme: "Catpuccin Mocha",
	}
	return sys
}

func MainQuotes() (map[int8]string){
	quotes := map[int8]string{
		1:"Your time is running out. Be yourself, be true",
		2:"Keep on faking, just to make it, what's the point of fixing unsolvable problems?",
		3:"The hurricane's eye is the quietest place you've ever been. Accept the chaos and let it be the peace you've deserved",
		4:"I recognize you, but I'm not afraid of you. Not anymore.",
		5:"Feelings are made to be felt. If you ignore them, they'll run after you, gaze at you in the eyes and say a simple 'why?'. Don't you ever judge them by their appeareance.",
		6:"Sometimes death is the only answer, so we can be reborn again.",
		7:"Pressing the same key eventually generates an error, Clear is bettter than clever.",
		8:"You are the universe experiencing itself, so are people around you. Harm anything and you've been harmed. ",
		9:"Light needs Darkness to exist.",
		10:"You may not be as cool as them, pretty as them but who said it's about being someone else? Happiness hides where your soul rests: the truth.",
		11:"The road is rough, take a rock and throw it in the river.",
		12:"Time abides no reason, yet brooks not a second to be reclaimed.",
		13:"Death comes for us all, enjoy your journey; every foreigner need a land to rest.",
	}
	return quotes
}

func GetFavoriteGames() []string{
	justChilling:= []string{
		"Fnaf: Five Nights At Freddy's",
		"Red Dead Redemption [never played :( ]",
		"Roblox [Not favorite, but it's good enough]",
		"Valorant [Used to play on Windows, but I keep up with the community]",
		"Mobile Legends",
		"Honor of Kings",
		"Arena of Valor",
	}
	return justChilling
}
func main() {
	fmt.Println("Guys I LOVE Golang btw")

    // random thought
    quotes := MainQuotes()
    rand.Seed(time.Now().UnixNano())
    randomID := int8(rand.Intn(len(quotes)) + 1)
    fmt.Println("---- Thoughts ----")
    fmt.Printf("\"%s\"\n\n", quotes[randomID])

    // I am Rafael!
    fmt.Println("---- Profile ----")
    ThisIsMe()

    // Learning
    fmt.Printf("\nStatus: %s\n", CurrentStats())
    fmt.Printf("Skill Level: %s\n", SkillLevel_Goal(50)) // Exemplo com 50 horas

    // Setup
    setup := SetupSpec()
    fmt.Printf("\nOS: %s | Theme: %s\n", setup.OS, setup.Theme)
    fmt.Print("Editors: ")
    for _, ed := range setup.Editor {
        fmt.Printf("[%s] ", ed)
    }
    fmt.Println()

    // Music
    fmt.Println("\n---- Music Taste ----")
    for _, s := range MusicTaste() {
        if s.Artist != "" {
            fmt.Printf("• %s (%s)\n", s.Artist, s.Genre)
        }
        for _, o := range s.Obs {
            fmt.Printf("  Note: %s\n", o)
        }
    }
	fmt.Println("\n---- Games ----")
	for _, game := range GetFavoriteGames() {
		fmt.Println(game)
	}
} // Since this file owns a main() function, you can run it whenever you want to.
```
How rude of me! I haven't talked to you guys since this whole code appeared! Well. Honestly, I'm aiming to join college when I finish High School, I have a bunch of dreams and goals.
What am I saying? Everyone's got this. Well, I made this GitHub profile just to play a lil bit so don't take it seriously. This is totally unprofessional (I'm not a professional)
Hope you guys enjoy my profile and my README, it took such a long time to write! 

The code is very basic, but it's honest. I don't know much about Golang and its features so far, but I tried to tell my story!
