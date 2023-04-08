# Zigzag
A zigzag is a pattern made up of small corners at variable angles, though constant within the zigzag, tracing a path between two parallel lines; it can be described as both jagged and fairly regular. 


        import time
        import sys
        space = 0 # How many spaces to indent
        space_increasing = True # Whether the indentation is increasing or not
        try:
            while True : # The main program loop
                print(' ' * space, end='')
                print('********')
                time.sleep(0.1) # Pause for 1/10 of a second
                if space_increasing :
                    space = space + 1 # Increase the number of spaces
                    if space == 20 :
                        space_increasing = False  # Change direction
                else:
                    space = space - 1 # Decrease the number of spaces
                    if space == 0:
                        space_increasing = True # Change direction
        except KeyboardInterrupt:
            sys.exit()

