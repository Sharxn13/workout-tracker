# Workout Tracker

![https://media.giphy.com/media/SdW7SEleK00Ug/source.gif](https://media.giphy.com/media/SdW7SEleK00Ug/source.gif)

Create an app that tracks your workouts.

##### Create a table

| id  | distance | name       |
| --- | --------:| ---------: |
|  1  |  2       | easy       |
|  2  |  2       | to work    |
|  3  |  20      | banana     |
|  3  |  20      | distance   |


##### Enter a run workout

```bash
$ node index.js 5.7 hard
```

##### See your planned workouts

```bash
$ node index.js
```

```

1. [ ] - 5.7km - easy run
2. [ ] - 6.8km - up a mountain
3. [ ] - 9.2km - banana
```



#### Further

Change your database. Add a column. When the run is completed, add a time.

```bash
$ node index.js complete 1 24.5
```

```
| id  | distance | name       | time  |
| --- | --------:| ---------: |:-----:|
|  1  |  2       | easy       | 12    |
|  2  |  2       | hard       | 5     |
|  3  |  20      | distance   | 6     |
|  4  |  20      | distance   |       |
```

```bash
$ node index.js
```

```
1. [ ] - 5.7km 
2. [ ] - 6.8km
3. [x] - 9.2km - 4:00
```

###### (Complete any of the below furthers in any order)

#### Further

In the output of your runs, output a pace.

```bash
$ node index.js
```

(these are listed in minute per km pace)
```
1. [ ] - 5.7km - 12:00
2. [ ] - 6.8km - 13:00
3. [x] - 9.2km - 4:00  - 10:00 m / km
```

#### Further
Add a stats functionality that gives the average time of all runs.

(You can do this with a SQL query, but calculating the average in javascript is just as good for now.)

#### Further
Add a stats functionality that gives the average distance of all runs.

#### Further
Add a functionality that gives the rating of the pace of a run "fast", "slow", "olympic record!!", etc.

Research running pace, or use this link: [https://www.verywellfit.com/walking-and-running-pace-and-speed-calculator-3952317](https://www.verywellfit.com/walking-and-running-pace-and-speed-calculator-3952317)


#### Further
Add a column named `created_at` with data type date and display the date the item was added. Look ahead in the gitbook for how to format the date type with `pg` library [https://wdi-sg.github.io/gitbook-2019/04-databases/postgres/sql-working.html](https://wdi-sg.github.io/gitbook-2019/04-databases/postgres/sql-working.html)


#### Further
Add a stats functionality to give you an average time / distance of runs for a given period of time.

```bash
$ node index.js average '2/3/2019' '1/5/2019'
```

You may want to look ahead in the gitbook for how to work with sql dummy data, a `seed.sql` file: [https://wdi-sg.github.io/gitbook-2019/04-databases/postgres/sql-working.html](https://wdi-sg.github.io/gitbook-2019/04-databases/postgres/sql-working.html)

#### Further
Add the ability to get a list of completed runs ordered by time (ascending and descending)

#### Further
Add the ability to get a list of completed runs ordered by time (ascending and descending) **for a given time period**

#### Further
Add the ability to get a list of runs above or below a certain pace.

```bash
$ node index.js findruns below 4:30
```

#### Further
Add the ability to permanently delete an item.

#### Further
Add a column named `updated_at` with data type date and display the date the item was marked completed.

#### Further
Use an ascii art generator to add style to your app: [http://patorjk.com/software/taag](http://patorjk.com/software/taag) - here you could use the ES6 string interpolation syntax.

#### Further
Add the ability to keep track of different sports. Add `swim`, `bike` and `walk`. You'll have to add another column in your database in order to keep track of which type of activity is entered.

```bash
$ node index.js run 5.7 hard
```
