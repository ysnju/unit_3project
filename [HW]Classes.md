<img width="2046" alt="Screenshot 2022-02-24 at 2 34 11" src="https://user-images.githubusercontent.com/89366347/155374780-910d33fc-15d5-48e9-9aaa-1f25442e816c.png">

```py

'''
methods things we do with data
objects the data
attributes properties of data
'''
class Anime:
    def __init__(self,year:int,name:str,seasons:int,genre:str,author:str):
        self.year = year
        self.name = name
        self.seasons = seasons
        self.genre = genre
        self.author = author

    def __lt__(self,other):
        'which anime was made first'
        print("The anime you chose was made earlier than the other anime. True or False")
        a = self.year
        b = other.year

        return self.year<other.year

    def __add__(self, other):
        'number of seasons'
        print("total seasons you would watch by watching these 2 anime")
        a = self.seasons
        b = other.seasons
        return self.seasons+other.seasons

    def __contains__(self, item):
        'check if genre is the same'
        print("any common genre in these two anime T/F")
        #O_genre for original genre
        #C_genre for compared genre
        O_genre = self.genre
        C_genre = item.genre

        common = O_genre.__contains__(C_genre)
        return common

    def length(self):
        'total min to watch the anime'
        print(f"{self.name} has {self.seasons} seasons. Taking you aprox {self.seasons*0.5*12} hours to fully watch")

    def past(self):
        print(f"the anime {self.name} was made {2022-self.year} years ago")



class Movies:
    def __init__(self,year:int,name:str,seasons:int,genre:str,director:str):
        self.year = year
        self.name = name
        self.seasons = seasons
        self.genre = genre
        self.director = director

    def __lt__(self, other):
        'which movie was made first'
        print("The movie you chose was made earlier than the other anime. True or False")
        a = self.year
        b = other.year

        return self.year < other.year

    def __add__(self, other):
        'number of seasons'
        print("total seasons you would watch by watching these 2 movies")
        a = self.seasons
        b = other.seasons
        return self.seasons + other.seasons

    def __contains__(self, item):
        'check if genre is the same'
        print("any common genre in these two movie T/F")
        # O_genre for original genre
        # C_genre for compared genre
        O_genre = self.genre
        C_genre = item.genre

        common = O_genre.__contains__(C_genre)
        return common

    def length(self):
        'total min to watch the anime'
        print(
            f"{self.name} has {self.seasons} seasons. Taking you aprox {self.seasons * 2} hours to fully watch")

    def past(self):
        print(f"the movie{self.name} was made {2022 - self.year} years ago")


class Animemovie(Movies):

    def length(self):
        print(f"{self.name} has {self.seasons} seasons. Taking you aprox {self.seasons * 2*12} hours to fully watch")

    def __lt__(self, other):
        'which anime movie was made first'
        print("The animemovie you chose was made earlier than the other animemovie. True or False")
        a = self.year
        b = other.year

        return self.year < other.year

    def __add__(self, other):
        'number of seasons'
        print("total seasons you would watch by watching these 2 anime movies")
        a = self.seasons
        b = other.seasons
        return self.seasons + other.seasons

    def __contains__(self, item):
        'check if genre is the same'
        print("any common genre in these two animemovies T/F")
        # O_genre for original genre
        # C_genre for compared genre
        O_genre = self.genre
        C_genre = item.genre

        common = O_genre.__contains__(C_genre)
        return common

    def past(self):
        print(f"the anime movie {self.name} was made {2022-self.year} years ago")
)


anime1 = Anime(year=2013,name="Attack on Titan",seasons = 6,genre = "Dark Exciting",author="Hajime Isayama")
anime2 = Anime(year=2018,name="Hozuki's Coolheadness",seasons = 8,genre = "Absurd",author="Natsumi Eguchi")
print(anime1.__lt__(other= anime2))
print(anime1.__add__(other=anime2))
print(anime1.__contains__(item=anime2))
anime1.length()

movie1 = Movies(year=2010,name="キングズマン",seasons = 3,genre = "action",director="コリンファース")
movie2 = Movies(year=2016,name="シンゴジラ",seasons =5,genre = "SF",director="庵野秀明")
print(movie1.__lt__(other= movie2))
print(movie1.__add__(other=movie2))
print(anime1.__contains__(item=movie2))
anime1.length()

```
