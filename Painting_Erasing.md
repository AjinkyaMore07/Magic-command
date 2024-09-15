# Basic Operations

    Painting:
        With Mouse:
            Position the box over the area you want to paint.
            Move the cursor over the color you want to use.
            Click the middle mouse button to paint.
        With Command:
            Use :paint layers, where layers is a list of layer names you want to paint.

    Erasing:
    
        With Mouse:
            Place the box over the area you want to erase.
            Move the cursor over a blank spot.
            Click the middle mouse button to erase.
        With Command:
            Use :erase layers, where layers is a list of layer names you want to erase.
        Using Macro ˆD:
            Position the box over the area to be erased.
            Move the cursor over a splotch of paint containing the layer(s) you want to erase.
            Press ˆD (Control-D) to erase those specific layers.


# Layer Interactions

    Transparent Combination: Some layers are transparent, so painting one on top of another will show a combination of both layers. For example, painting metal1 (blue) on top of polysilicon (red) results in a combined effect.

    Different Outcome: Painting one layer on top of another may result in a different layer or effect. For example, painting poly on top of ndiff produces ntransistor.

    Replacement: Some layers replace others when painted on top. For example, painting pcontact on top of ntransistor replaces the ntransistor layer with pcontact.


# Practice Tips

    Experiment with Layer Combinations:
        Try painting different layers on top of each other to see the combined or resultant effects.
        Use :paint command for specific layers and observe the results.

    Erase with Precision:
        Use the ˆD macro to erase specific layers without affecting others.
        Practice using ˆD on areas with multiple layers to get a feel for how it interacts with different layer combinations.

    Reset if Necessary:
        If you make a mistake or the screen gets messed up, restart Magic to reset the environment.

    Design Rule Violations:
        Ignore white dots (design rule violations) for now; they will be explained in a later tutorial.


# Commands and Macros Recap

    Paint: :paint layer1,layer2,...
    Erase: :erase layer1,layer2,...
    Erase Specific Layers: ˆD (Control-D)
    Erase All: ˆD over empty space
