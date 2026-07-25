# ML Learning Path

A complete Data Science & Machine Learning learning path — from Python basics to advanced interview preparation.

## Structure

### ML_Learning_Path/
Sequential notebooks from beginner to advanced. Study in order.

| # | Notebook | Topics |
|---|---|---|
| 00 | Start Here Index | Overview and study guide |
| 01 | Python Basics | Variables, functions, comprehensions, OOP |
| 02 | NumPy Fundamentals | Arrays, broadcasting, linear algebra |
| 03 | Pandas Data Analysis | DataFrames, GroupBy, merge, time series |
| 04 | Data Visualization | Matplotlib, Seaborn, chart types |
| 05 | Exploratory Data Analysis | EDA framework, outliers, distributions |
| 06 | Feature Engineering | Encoding, scaling, imputation, pipelines |
| 07 | Linear Regression | OLS, Ridge, Lasso, polynomial regression |
| 08 | Logistic Regression | Classification, ROC, precision-recall |
| 09 | Decision Trees & Random Forests | Gini, entropy, feature importance |
| 10 | SVM & KNN | Kernels, margins, distance metrics |
| 11 | Gradient Boosting & XGBoost | Boosting, learning rate, early stopping |
| 12 | Clustering | K-Means, DBSCAN, hierarchical |
| 13 | Dimensionality Reduction | PCA, t-SNE, explained variance |
| 14 | Model Selection & CV | K-Fold, stratified, time series split |
| 15 | Neural Networks | MLP, activation functions, backprop |
| 16 | Time Series | ARIMA, stationarity, lag features |
| 17 | NLP & Text Analysis | TF-IDF, LDA, sentiment analysis |
| 18 | End-to-End ML Project | Full pipeline: EDA → model → deploy |
| 19 | Advanced Topics | Ensembles, anomaly detection, SHAP |

### ML_Learning_Path/Advanced_Notebooks/
Deep-dive interview preparation notebooks.

| # | Notebook | Key Topics |
|---|---|---|
| 01 | Advanced Python Interview | Generators, decorators, OOP traps, 15 interview traps |
| 02 | Advanced NumPy Interview | Views vs copies, einsum, broadcasting rules |
| 03 | Advanced Pandas Interview | SettingWithCopyWarning, groupby internals, performance |
| 04 | Statistics & Probability Interview | CLT, A/B testing, Bayes, Simpson's paradox |
| 05 | ML Concepts Interview | Bias-variance, data leakage, gradient descent |
| 06 | Feature Engineering Advanced | MCAR/MAR/MNAR, VIF, cyclical encoding |

### ML_Interview_Implementations/
Real implementation notebooks based on top ML resources.

| # | Notebook | Source Inspiration |
|---|---|---|
| 01 | Math & Statistics Interview | Chip Huyen ML Interviews Book Ch.5 |
| 02 | Classical ML Deep Dive | Hands-On ML algorithms from scratch |
| 03 | Deep Learning PyTorch | PyTorch deep learning with numpy fallbacks |
| 04 | NLP & Transformers | Attention from scratch, transformer encoder |
| 05 | MLOps & Production ML | Drift detection, A/B testing, experiment tracking |
| 06 | ML System Design | Fraud detection, recommendation engine, FAANG Q&As |
| 07 | Computer Vision | HOG, IoU, NMS, ResNet skip connections |
| 08 | Kaggle Competition Strategies | Stacking, Optuna tuning, pseudo-labeling |
| 09 | How Search Works | Exact match, TF-IDF, semantic embeddings, visualisation of search spaces |

## How to Run

```bash
# Start Jupyter server
python3 -m jupyter notebook --no-browser --port=8888 --ip=0.0.0.0 \
  --ServerApp.token='' --ServerApp.password=''

# Open in browser
# http://localhost:8888
```

All notebooks have pre-executed outputs saved — no need to run them to see results.

## Study Plan

See `ML_Learning_Path/STUDY_PLAN.txt` for a complete printable study plan with time estimates and daily schedule.

## Requirements

```
numpy pandas matplotlib seaborn scikit-learn scipy
statsmodels xgboost imbalanced-learn shap tensorflow
```

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy \
  statsmodels xgboost imbalanced-learn shap tensorflow
```

### SystemDesign/
60-day system design series — one notebook per day, architecture diagrams + bottleneck analysis.

| Day | Notebook | Topic |
|---|---|---|
| 01 | Day01_Single_Server_Setup | Single server architecture, request flow, bottlenecks, scaling triggers |
| 02 | Day02_Database_Separation | Web tier vs data tier split, SQL vs NoSQL, four NoSQL models, decision framework |
| 03 | Day03_Load_Balancer | Load balancer architecture, 4 routing algorithms, vertical vs horizontal scaling, failover, auto-scaling |
| 04 | Day04_Database_Replication | Master-Slave replication, sync/async/semi-sync modes, failover promotion, read/write split, trade-off analysis |
| 05 | Day05_Cache | Cache hit/miss flow, Read-Through/Write-Through/Write-Behind/Cache-Aside strategies, TTL, LRU/LFU eviction, consistency, SPOF |
| 06 | Day06_CDN | Global CDN architecture, 6-step workflow, latency impact, TTL lifecycle, invalidation, Pull vs Push CDN, provider landscape |
| 07 | Day07_Stateless_MultiDC | Stateful sticky-session problem, stateless shared store, autoscaling, multi-data-center with GeoDNS, cross-DC replication, failover |
| 08 | Day08_Data_Centers | GeoDNS resolution flow, traffic split x%/(100-x)%, DC outage failover sequence, data sync strategies, RTO/RPO, multi-DC deploy pipeline |
| 09 | Day09_Message_Queue | Producer→queue→consumer architecture, async vs sync decoupling, photo processing use case, worker autoscaling by queue depth, fan-out/pub-sub, priority queue, dead-letter queue, RabbitMQ vs Kafka vs SQS vs Redis Streams |
| 10 | Day10_Database_Sharding | Horizontal data-tier scaling, hash-based shard routing, shard key selection criteria, resharding with consistent hashing, celebrity/hotspot key problem, cross-shard JOIN problem, denormalisation, range/hash/directory/geo sharding strategies |
| 11 | Day11_Rate_Limiter_Part1 | Rate limiter concept and HTTP 429 flow, client vs server vs API gateway placement, distributed RL with Redis atomic counters, six design requirements mapped to architecture decisions, server-side vs gateway decision guide |
| 12 | Day12_Rate_Limiter_Part2 | Token bucket (Amazon/Stripe), leaky bucket (Shopify), fixed window counter with boundary spike problem, sliding window log with Redis sorted sets, sliding window counter hybrid algorithm, 5-algorithm comparison matrix |
| 14 | Day14_URL_Shortener | Base62 encoding (62^7=3.5T), 301 vs 302 redirect, DynamoDB TTL, LRU cache design, Kinesis analytics pipeline, AWS Lambda+CloudFront architecture |
| 13 | Day13_Rate_Limiter_Part3 | Redis INCR/EXPIRE counter store, rules-on-disk with worker cache, drop vs enqueue handling, full sequence diagram, race condition fix with Lua scripts, synchronisation fix with centralised Redis, complete architecture (Mermaid diagrams) |
