Divers_rugos <- renyi_df %>%
filter(Q == 1)
head(Divers_rugos)
Divers_rugosP <- ggplot(Divers_rugos, aes(x = VerRelief, y = Value)) +
geom_point() +
theme_classic() +
labs(x = "LogVR", y = "Effective diversity (Hill number Q = 1)")  + geom_smooth(method = "lm", se = TRUE) +  # Add linear regression line with 95% confidence interval
  labs(x = "X Axis Label", y = "Y Axis Label", title = "Scatterplot with Linear Regression Line")  # Add axis labels and title

Divers_rugosP

