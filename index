import turtle

def draw_tree(branch_length, t):
    # Base case: stop when the branch gets too small
    if branch_length < 5:
        return
        
    t.forward(branch_length)
    t.right(20)
    draw_tree(branch_length - 15, t) # Draw right branch
    
    t.left(40)
    draw_tree(branch_length - 15, t) # Draw left branch
    
    t.right(20)
    t.backward(branch_length)        # Return to starting node

# Setup the screen and turtle
t = turtle.Turtle()
t.screen.bgcolor("black")
t.color("cyan")
t.speed("fastest")

# Position the turtle at the bottom center, pointing up
t.left(90)
t.up()
t.backward(150)
t.down()

# Start the recursion
draw_tree(80, t)
turtle.done()