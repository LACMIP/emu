---
title: Troubleshooting
navcat: Basic Info
tags:
---

Problem: EMu tells me "TexAPI Error: Cannot get host information (Number 304)" or "Cannot send to remote host (Number 310)." Solution: To solve the error, go to ‘START -> ALL PROGRAMS -> ACCESSORIES ->COMMAND PROMPT’ in Marconi. You will see a black box with a ‘c: \documents and Settings\’  prompt. Type ‘taskmgr’ and press enter. The windows task manager will appear, with several tabs at the top.  The first is APPLICATIONS.  Do you see EMU running there?  If so, CLICK on it once (to highlight it) and then click END TASK at the bottom. If EMu is not listed there, click on processes to see if it is listed there.  Again, if so, highlight it and click END PROCESS. This problem occurs because EMu needs to be shut down properly whenever you exit Marconi, otherwise it remains running in the background. Even if Marconi logs you off automatically, you should sign back in to properly exit EMu. If you have been doing so, then the error is likely the result of a network or server issue--in this case, note the time and relay this information to Bill or IT.

##

Problem: EMu says “TextAPI Error: Can’t open file /home/emu/lacm/loads/fifo/input. Fifo call failed. Expression failed. Validation failed. (Number -4)”. EMu is undergoing maintenance. Occurs on Saturdays.

##

Problem: EMu error Number 310. It was likely a network error.  I have not seen that specific error number while using EMu, but it is typically related to querying a remote system.  My guess is there was a momentary network disconnect while your volunteer was in EMu.

##

Problem: EMu error when you try to delete a record says “attached to Taxonomy.” You need to delete a record.
