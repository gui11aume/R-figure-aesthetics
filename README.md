# R-figure-aesthetics
```R
set.seed(123)
x = rnorm(20)

pdf("plot-1.pdf")
par(mar=c(3.1,3.1,0,0))
plot(x, panel.first=grid(),
     bty="n", ylab="", xlab="", xaxt="n", yaxt="n", type="n")
lines(x, lwd=2, col="gray20")

axis(side=1, col="gray30", cex.axis=.8, padj=-.9, col.axis="gray20")
axis(side=2, col="gray30", cex.axis=.8, padj= .9, col.axis="gray20")
title(xlab="x value (unit)", line=2, col.lab="gray30")
title(ylab="y value (unit)", line=2, col.lab="gray30")
dev.off()
```
<img src="plot-1.png" alt="Plot #1" width="600"/>
