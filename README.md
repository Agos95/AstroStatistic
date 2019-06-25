# Analysis of Kepler mission lightcurves

Let us perform some of the autoregressive modeling analysis of two Kepler stars discussed by [Caceres et al., 2019](https://arxiv.org/abs/1901.08003).

1. Provide basic information about the lightcurves: length, `NA` fraction, IQR and other quantiles, autocorrelation function, and time series diagnostics (Ljung-Box, Durbin-Watson, augmented Dickey-Fuller, Anderson-Darling tests).
2. Smooth lightcurves, with confidence bands, and interpolate gaps. Try `LOESS`, `COBS`, `locfit`, and `imputeTS`. Calculate residuals from a smoothed function with time series diagnostics.
3. `ARIMA` modeling. Try individual model orders using R's arima function, and try automatic model selection using `CRAN` forecast's `auto.arima (stepwise=FALSE)`. Perform time series diagnostics on the residuals.
4. Periodicity search. Try the functions in `CRAN`'s RobPer as well as `R`'s Fourier spec.pgram. Any planets?