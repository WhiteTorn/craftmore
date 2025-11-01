

This repository consists two folders

1. CraftMore - fork of [Building Makemore](https://youtube.local/watch?v=PaCmpygFfXo&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&index=1) Tutorial. [Original Repo](https://github.com/karpathy/makemore/tree/master)

2. CraftGeo - Georgian version of Craftmore. data consists of 60k georgian names and **Makemore** (trigram) tries to generate new names based on it. files required to be cleared, correctly loaded in the 3 Dimensional Tensor and best possible hyperparameters to train the model
   - L2 = 0.0001 (Less just decreased by tiny amounts)
   - Learning Rate = 50 (Less not worked, more not tested)
   - Steps = 2000 (More  gave better results but execution time exceeded 10 minutes and more for single train, decreased loss was not worth time)
  
   - Results: Makemore perfomed on georgian dataset worse than on english, cause dataset consisted more examples, and more characters for tensor. makemore is too weak for names. MLP in part 2 I think should work 2x better.
