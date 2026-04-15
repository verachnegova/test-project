|Bug ID|Title|Severity|Reproduction Steps|Expected vs Actual result|Business Impact|Evidence|Test ID|
| ---: | --- | --- | --- | --- | --- | --- | --- |
|1|Modal window displays incorrect bet details|Crit|1. Make a selection, enter a stake within user's balance.<br>2. Press "Place Bet" button.<br>3. Check modal and compare it with Place a bet API response.|3. Modal contains:<br> * Title "Bet Placed Successfully!" - **PASS**,<br> * Bet ID - **PASS**,<br> * Match details - **FAIL: the teams are mixed up in the matchId, kick-off date is not displayed**,<br> * Selection - **FAIL: selection is not displayed**,<br> * Stake - **PASS**,<br> * Odds at placement - **PASS**,<br> * Potential payout - **FAIL: incorrect value of Potential payout**,<br> * Placement timestamp - **PASS**,<br> * Close button - **PASS**. |Incorrect data about bets placed misleads users, increases the number of support requests, and negatively impacts the product's rating.|![Place a bet API response:](img/Place_bet_response.jpg)<br><br>![Modal:](img/Place_bet_modal.jpg) |6|
|2||||||||
|3||||||||
|4||||||||
|5||||||||
|6||||||||
