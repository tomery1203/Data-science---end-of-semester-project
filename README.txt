Data Science Project:

By:Tomer Yaish, Dan Kvitca

Subject: prediciton of new video games success (success==selling more than 1,000,000 copys)
Language: Python 100%
libraries:Pandas,Numpy,Seaborn,Matplotlib,Yellowbrick for Sickilearn,Sickitlearn,BeautifulSoup




Genreal:
This project is divided to four parts:
1. data mining: we created 3 crawlers.
	MetaCrtic:
		'name':[], 'release date':[], 'developer': [], 'genre':[], 'rating':[], 'user rating':[],'age':[],'platforms':[],'number of players':[],'publisher':[]
		after mining this data, we saved it to a dataframe.
	VgChartz:
		sales_list=[] ('total sales/mil')
		
	PriceCharting:
		prices_list=[] ('price)

2. Data Cleaning:
	handling nan values,
	droping values,
	outliers,
	modifying strings:
		genre- was split to be only the main genre (for example: from metacritic-"Action/Shooter/OpenWorld" to- "Action")
		number of players - there wore alot of multiplycation in data. for example: 2 players was at some index "2", and 
		at other index "2 players". now all values are integers.
	hit column (For ML) - we added a hit collumn, if a game sold more than 1,000,000 copys than 1. else 0.
3) Data Visualization:
	conection_between_rating_to_sales
	conection_between_user_rating_to_sales
	most_selling_dev
	most_selling_pub
	biggest_dev_by_games
	most_popular_game_genre
	best_user_score_by_dev
	best_score_by_dev
	best_score_by_platform
	best_user_score_by_platform

4) Machine-Learning:
	method -RandomForrestClassifier.
	lowest acu measured- 83.4
	