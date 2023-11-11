# Weather CLI - Sample

Adapted from [How to create your own .NET CLI tools to make your life easier
](https://www.youtube.com/watch?v=JNDgcBDZPkU) by Nick Chapsas.


# Install

To install, run `sh install.sh` from the cloned repo main folder.

# Pack

To pack this as a nuget package, run `dotnet pack`, or for convenience, run `sh lazypack.sh`.

I recommend using `lazypack` so you can make tests to your updates more frequently and not have to memorize the commands.

# Uninstall

To uninstall, run `sh uninstall.sh`.

# Troubleshooting

If you clone this repo, be sure to name your project after the command you wish to type, e.g. `dotnet run weather` or `weather` will expect the project to be named `weather`.

If you name your namespace differently (in my case, it is `weather.cli`), be sure all of your `.cs` files reflect this.  You can `ls` into your `./nupkg` folder to verify the namespace matches your code.  If there's a mismatch, the `dotnet tool install` will complain!

