# IPB
David Roberts, Pawel Kwiatkowski

Rule 1) If no action is made within any step requiring action within 5 minutes, either initiate lock down of card if valid card was inputted and return to Stage 1).

Stage 1) Input card card screen.
	Stage 1a) If card is valid, go to stage 2).
	Stage 1b) If card is invalid, return card.
	
Stage 2) Input PIN screen
	Stage 2a) If PIN is inputted correctly, go to stage 3).
	Stage 2b) If PIN is inputted incorrectly, go back to Stage 2). If repeated 3 times, initiate lock down of card and return to Stage 1)

Stage 3) Show menu. Fast Cash aka 50 zl without receipt/Change PIN/Regular Withdrawal, Show Balance, Show statement. Depending on chosen command, go to respective substage 3.
	Stage 3a) Fast Cash aka 50 zl without receipt. If chosen, proceed to stage 4).
	Stage 3b) Change PIN. If chosen, proceed to stage 3ba)
		Stage 3ba) Input current PIN.
			Stage 3baa) If inputted correctly, show new PIN menu. Inputted PIN becomes new PIN after acceptation and card is returned and return to Stage 1. If new PIN is rejected, return to Stage 3.
			Stage 3bab) If inputted incorrectly, go back to Stage 3ba). If inputted incorrectly 3 times, initiate lock down of card. 
	Stage 3c) Regular withdrawal. Show available denominations and custom denomination input. 
		Stage 3ca) Depending on chosen denomination, process card and charge account balance. Proceed to stage 4)
	Stage 3d) Show account balance. If chosen, show available account types. Proceed to stage 3da)
			Stage 3da) Depending on chosen account type, proceed to stage 4).
	Stage 3e) Show Statement. If chosen, show statement. Query for print.
		Stage 3ea) If yes, print statement. Return card and return to Stage 1)
		Stage 3eb) if no, return card and return to Stage 1).
	Stage 3f) Money transfer.
		Stage 3fa) User chooses first account, from which funds are to be transferred from. Proceed to stage 3fb)
		Stage 3fb) User choosed second account, to which funds are to be transferred to. Proceed to stage 3fc)
		Stage 3fc) Input amount. Proceed to stage 4) 	
	Stage 3g) Money deposit.
		Stage 3ga) Choose deposit account.
			Stage 3gaa) After choosing, input money. 
				Stage 3gaaa) When money is inputted, ATM counts the money. Display inputted money. Verify funds inputted total with user.
					Stage 3gaaaa) If more money is to be inputted, return to Stage 3gaaa)
					Stage 3gaaab) If total is accepted, go to Stage 4).
					Stage 3gaaac) If not accepted, return bills and return to stage 3).
				Stage 3gaab) Reject invalid bills. Return to Stage 3gaaa)
				
Stage 4) Verify chosen action with bank.
	Stage 4a) If verification successful, go to respective stage.
		Stage 4aa) Stage 5a in case of withdrawal
		Stage 4ab) Stage 5b in case of account balance
		Stage 4ac) Stage 5c in case of money transfer.
		Stage 4ad) Stage 5d in case of money deposit.
	Stage 4b) If verification is unsuccessful, return reason of verification being unsuccessful and return to Stage 3)

Stage 5a) In case of withdrawal, ask for account type. 
	Stage 5aa) When chosen, ask receipt option. Proceed to stage 5aaa)
		Stage 5aaa) Dispense previously chosen amount of funds. Print receipt if chosen. Return card. Return to Stage 1)
Stage 5b) In case of account balance, show account balance and ask for account balance print. If print is chosen, proceed to stage 5ab)
	Stage 5ba) Print account balance. After printing, ask for additional transaction. 
		Stage 5baa) If yes, go to Stage 3)
		Stage 5bab) If no, return card and go to Stage 1)
Stage 5c) If successful, show new account balance for both accounts. Ask for print.
	Stage 5ca) If yes, print and return card, Return to Stage 1)
	Stage 5cb) If no, return card. Return to Stage 1).
Stage 5d) Show new account balance. Ask for print of current account balance.
	Stage 5da) If yes, print and return card, Return to Stage 1)
	Stage 5db) If no, return card. Return to Stage 1).
