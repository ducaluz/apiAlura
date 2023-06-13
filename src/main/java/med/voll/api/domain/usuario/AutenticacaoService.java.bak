package med.voll.api.domain.usuario;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.security.core.userdetails.UserDetails;
import org.springframework.security.core.userdetails.UserDetailsService;
import org.springframework.security.core.userdetails.UsernameNotFoundException;
import org.springframework.stereotype.Service;

@Service
public interface AutenticacaoService implements UserDetailsService  {

    @Autowired
    private UsuarioRepository repository; 

    @Override
    public UserDetails loUserByUsername(String username) throws UsernameNotFoundException {
        return repository.findByLogin(username); 
    }
}
