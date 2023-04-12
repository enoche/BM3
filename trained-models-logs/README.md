We share the [trained models and logs](https://drive.google.com/drive/folders/1pFcT22yCNYmSeJZyGQRS0QtiG0APCNfi?usp=share_link) that reach the best performance under each dataset

## Trained Models & Logs
- [Baby@Google Drive](https://drive.google.com/drive/folders/1OmRY9Z9fC01HjzT1qDuUZEwUBq03oZ5s?usp=share_link): 385M
- [Sports@Google Drive](https://drive.google.com/drive/folders/12DngCZbMafipy2cpcWEyHz9kmKejOGcu?usp=share_link): 984M
- [Elec@Google Drive](https://drive.google.com/drive/folders/1QSojeVMGQvGsgNE5GD4T7ZA7ncllWU5N?usp=share_link): 3.34G

### Notes
Anyone can load the saved `checkpoints` of our models with the pytorch official instructions: https://pytorch.org/tutorials/beginner/saving_loading_models.html   
Here is how we save our model:
```
    def _save_checkpoint(self, epoch):
        r"""Store the model parameters information and training information.
        Args:
            epoch (int): the current epoch id
        """
        state = {
            'config': self.config,
            'epoch': epoch,
            'cur_step': self.cur_step,
            'best_valid_score': self.best_valid_score,
            'state_dict': self.model.state_dict(),
            'optimizer': self.optimizer.state_dict(),
        }
        torch.save(state, self.saved_model_file)
```
