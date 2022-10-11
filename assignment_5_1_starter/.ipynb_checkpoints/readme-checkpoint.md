{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "0519d223",
   "metadata": {},
   "source": [
    "# Readme.md\n"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "3bc2b77b",
   "metadata": {},
   "source": [
    "# Source dataset description\n",
    "* This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).\n",
    "* The initial dataset was 12684 rows and 26 columns\n",
    "* After removing columns with sparse data and row with Nulls, 12079 rows and 25 columns were left including: destination, passanger, weather, temperature, time, coupon, expiration, gender, age, maritalStatus, has_children, education, occupation, income, Bar, CoffeeHouse, CarryAway, RestaurantLessThan20, Restaurant20To50, toCoupon_GEQ5min, toCoupon_GEQ15min, toCoupon_GEQ25min,\tdirection_same, direction_opp, and Y\n",
    "\n",
    "# When limiting the data to Bar coupons, the following was observed:\n",
    "* Overall, people accepted the Bar coupon around 41% of the time.\n",
    "* People who go to the bar 4 or more times per month were much more likely to accept the coupons (76% vs. 37%)\n",
    "* For people who went more than once a month, age was not a factor in the acceptance rate.\n",
    "\n",
    "# When limiting the data to Coffee House Coupons, the following was observed: \n",
    "\n",
    "* Overall, people accepted the Coffee House coupon around 49% of the time.\n",
    "* People who had no urgent place to be, were a student, or had incomes below 75K were more likely to accept the coupon\n",
    "* Sales people who made more than 75K and were headed home were much more unlikely to accept the coupon (39%)\n",
    "* Students who made less than 75K and had no urgent place to be were more likely to accept the coupon (63%)\n",
    "\n",
    "# Possible Next Steps\n",
    "* Determine acceptance ratios for additional features such as education and marital status\n",
    "* Continue to identify the best performers individually, and then combine them with additional features to observe which ones perform the best together\n",
    "\n",
    "## The Jupyter Notebook used to analyze the data can be found at [prompt.ipynb](./prompt.ipynb)"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.12"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
