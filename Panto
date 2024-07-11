# Define the criteria and their descriptions with respective subscores
criteria = [
    {
        "name": "Dividend Income (Staking and Yield Farming)",
        "description": "Earn passive income through staking and yield farming opportunities.",
        "subcriteria": [
            {
                "name": "Staking",
                "description": "Earn rewards by participating in network staking.",
                "subscores": {
                    "Ease of Participation": 4,
                    "Rewards Competitiveness": 5,
                    "Security of Staking Mechanism": 3
                }
            },
            {
                "name": "Yield Farming",
                "description": "Provide liquidity to DeFi platforms for additional token rewards.",
                "subscores": {
                    "APY Offered": 4,
                    "Risk Associated with Platform": 3,
                    "Token Volatility in Farming": 3
                }
            }
        ]
    },
    {
        "name": "Capital Appreciation",
        "description": "Potential for token value appreciation based on project growth and market demand.",
        "subcriteria": {
            "Market Demand and Adoption": 5,
            "Project Innovation and Development": 4,
            "Historical Price Performance": 3
        }
    },
    {
        "name": "Ownership and Voting Rights (Governance Tokens)",
        "description": "Hold tokens to participate in project governance and decision-making.",
        "subcriteria": {
            "Voting Power Influence": 4,
            "Governance Transparency": 3,
            "Voter Participation Incentives": 2
        }
    },
    {
        "name": "Limited Liability",
        "description": "Investment risk limited to the amount invested, similar to traditional investments.",
        "subcriteria": {
            "Risk Management Features": 4,
            "Legal Protections for Investors": 3
        }
    },
    {
        "name": "Portfolio Diversification",
        "description": "Diversify investment portfolio by including digital assets alongside traditional assets.",
        "subcriteria": {
            "Correlation with Traditional Assets": 3,
            "Asset Class Diversity": 4
        }
    },
    {
        "name": "Potential Tax Benefits",
        "description": "Tax advantages associated with cryptocurrency investments.",
        "subcriteria": {
            "Tax Jurisdiction Benefits": 3,
            "Holding Period Advantages": 2
        }
    },
    {
        "name": "Access to Information",
        "description": "Transparent project updates and communications to keep investors informed.",
        "subcriteria": {
            "Frequency of Updates": 4,
            "Clarity of Communication": 3
        }
    },
    {
        "name": "Share Buybacks (Token Burns)",
        "description": "Token burns to reduce supply and potentially increase token value.",
        "subcriteria": {
            "Frequency and Magnitude of Burns": 4,
            "Market Impact and Perception": 3
        }
    },
    {
        "name": "Market Perception and News",
        "description": "Impact of market sentiment and news on token value.",
        "subcriteria": {
            "Positive News Frequency": 5,
            "Sentiment Analysis and Social Media Impact": 4
        }
    },
    {
        "name": "Analyst Recommendations (Influencer and Analyst Impact)",
        "description": "Influence of cryptocurrency analysts and influencers on market sentiment and investor behavior.",
        "subcriteria": {
            "Analyst Coverage Quality": 4,
            "Influencer Engagement and Endorsements": 5
        }
    },
    {
        "name": "Scarcity of Tokens (Limited Supply)",
        "description": "Impact of fixed or limited token supply on token economics and value.",
        "subcriteria": {
            "Total Supply versus Circulation": 5,
            "Tokenomics and Inflation Control": 4
        }
    }
]

# Function to calculate total scores for each criterion
def calculate_total_scores(criteria):
    total_scores = []
    for criterion in criteria:
        if isinstance(criterion['subcriteria'], list):
            # Calculate total score for subcriteria (e.g., Dividend Income)
            total_score = sum(sum(subcriterion['subscores'].values()) for subcriterion in criterion['subcriteria'])
        else:
            # Calculate total score for subcriteria (e.g., Capital Appreciation)
            total_score = sum(criterion['subcriteria'].values())
        
        total_scores.append({
            "name": criterion['name'],
            "total_score": total_score
        })
    
    return total_scores

# Example usage:
total_scores = calculate_total_scores(criteria)

# Print results
for score in total_scores:
    print(f"{score['name']}: Total Score = {score['total_score']}")
