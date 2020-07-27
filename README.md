# COVID19-PRM
Repo for COVID19 Political Realities Model (PRM)

The Political Realities Model (PRM) is built on observations of macro-level societal and political responses to COVID measured only in terms of infections and deaths. The starting point of the model is the belief that individuals' and policy makers' perceptions of COVID-19 risks generate a relatively narrow and fairly predictable, if not ideal, set of responses. Although specific individual behavior and government regulation may vary over time and from place to place, the range of what a society and its elected officials will accept can relatively easily be characterized. This model seeks to characterize these responses and models their impact on infection rates, which in turn is related to deaths via a simple (time- and geographically-varying) phenomenological model derived through fitting, which therefore builds in variation in the demographics of the infected population, access to health care & COVID testing and the infection fatality rate from place to place. At present the model is deterministic rather than probabilistic, and so only provides point forecasts. The model considers the United States at the state level.

This is very much a work in progress.

The phenomenological relationship between infections and deaths is, in the present version, a convolution of a normal distribution death curve centered at 20 days delay from reported infection with a sigma of 3 days weighted by a time- and geographically-carying case fatality rate (CFR) factor derived from fitting past data. State-level CFRs generally fall in the range of 0.015 to 0.025 as late July 2020. This approach could be modified by introducing flexibility in the shape of the death distribution curve (e.g., delay, width, skew) but this does not seem to be as important of a factor in the output of the model as the behavioral and policy choices (i.e., the "political choices.")

The "political choices" are modeled using a 3-level categorization of (7-day averaged) new infections per capita (low, medium and high). The categorization in turn affects changes in new infection rates in the model (forcing down or allowing to go up), with limits based on observations from prior data. The observed daily rate in change of the (7-day averaged) new infections is rarely below 0.98 at the current time, but there is considerably more headroom above 1.0.

New developments will be described here. 

A more detailed explanation of methods will follow.
