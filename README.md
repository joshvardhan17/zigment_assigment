let score = 0;

// Scoring criteria
if (inputData.companySize === "1-50 employees") score += 10;
else if (inputData.companySize === "51-200 employees") score += 20;
else if (inputData.companySize === "201-1000 employees") score += 30;
else if (inputData.companySize === "1000+ employees") score += 40;

if (inputData.budget === "Less than $10,000") score += 5;
else if (inputData.budget === "$10,000 - $50,000") score += 15;
else if (inputData.budget === "$50,001 - $100,000") score += 25;
else if (inputData.budget === "More than $100,000") score += 35;

if (inputData.industry === "Technology") score += 20;
else if (inputData.industry === "Finance") score += 15;
else if (inputData.industry === "Healthcare") score += 25;
else if (inputData.industry === "Retail") score += 10;
else if (inputData.industry === "Other") score += 5;

if (inputData.urgency === "Immediate") score += 30;
else if (inputData.urgency === "Short-term") score += 20;
else if (inputData.urgency === "Medium-term") score += 10;
else if (inputData.urgency === "Long-term") score += 5;

return { leadScore: score };
