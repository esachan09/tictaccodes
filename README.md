# tictaccodes
import pyttsx3 as p

engine = p.init()

engine.say("hello world. my name is sexyshane ang ganda ganda ko")
engine.runAndWait()




game = [[0,0,0],
		[0,0,0],
		[0,0,0],]

def game_board(game_map, player=0, row=0, column=0, just_display=False):
	print ("   a  b  c")
	if not just_display:
		game_map[row][column] = player 
	for count, row in enumerate(game_map):
		print(count, row)
	return game_map


game = game_board(game, just_display=True)
game = game_board(game,player=1, row=2, column=1)
