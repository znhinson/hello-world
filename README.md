def winner(board):
    #r represents the rows in the 2 dimensional matrix
    #will iterate three times for each case: horizontal and vertical
    #two separate case statements for the case in which there is a diagonal win
    for (int r = 0; r < 3; r++) { #for loop that iterates to find any horizontal/vertical wins for X or O

        if (board[r][0] == board[r][1] == board[r][2]) { 
            winner = board[r][0]; #returns winner as X or O
        }

        if (board[0][r] == board[1][r] == board[2][r]) {
            winner = board[0][r];
        } else if (board[2][0] == board[1][1] = board[0][2]) { #determines any diagonal wins , returns winner as X or O
            winner = board[2][0];
        } else if (board[0][0] == board[1][1] = board[2][2]) {
            winner = board[0][0];
        } else{
            raiseNotImplementedError; #no winner has been discovered, or there is a tie
            
    def terminal(board):
     winner(board);
     for (int r = 0; r < 3; r++) {
     if(winner==board[r][0]||winner==board[0][r]||winner==board[0][0]||winner==board[2][0]){
        return True;
     }else{
     return False;
     
    """
    Returns True if game is over, False otherwise.
    """
    raise NotImplementedError


def utility(board):
    """
    Returns 1 if X has won the game, -1 if O has won, 0 otherwise.
    """
    raise NotImplementedError
