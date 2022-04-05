from discord.ext import commands

bot = commands.Bot(command_prefix="!")

def has_numbers(inputString):
  return any(char.isdigit() for char in inputString)

@bot.event
async def on_ready():
    print("Ready!")

@bot.command(name='math')
async def test(ctx, arg):
    if has_numbers(arg):
      math = eval(arg)
      if math == True:
        await ctx.send("Answer: Correct")
      elif math == False:
        await ctx.send("Answer: Incorrect")
      else:
        await ctx.send(math)
    else:
      await ctx.send("Couldn't answer")
bot.run(TOKEN HER)
