## Dataset Description : 

- the Train dataset, which you will use to train your algorithm
- the Xtest dataset, for which you will need to predict the column 'target'

The dataset has the following columns:
- flight_date : the date of the flight
- from: the code of the departure airport
- to: the code of the arrival airport
- avg_weeks: the average number of weeks between ticket purchase and flight date
- std_weeks: the standard deviation of the number of weeks between ticket purchase and flight date
- target: the variable to predict. It relates to the number of passengers on the flight. For reasons of privacy, the number of passengers is not available, and the 'target' variable is available instead.

Each row corresponds to one flight.

The data is compressed with the bzip2 format. You can load it to Pandas 🐼 with:
train = pd.read_csv('./data/flights_train.csv.bz2')
X_test = pd.read_csv('./data/flights_Xtest.csv.bz2')
